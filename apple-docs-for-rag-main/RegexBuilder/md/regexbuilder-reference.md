

- RegexBuilder
-  Reference 

Structure

# Reference

A reference to a captured portion of a regular expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Reference
```

## Overview

You can use a `Reference` to access a regular expression, both during the matching process and after a capture has been successful.

In this example, the `kind` reference captures either `"CREDIT"` or `"DEBIT"` at the beginning of a line. Later in the regular expression, the presence of `kind` matches the same substring that was captured previously at the end of the line.

```
let kindRef = Reference(Substring.self)
let kindRegex = ChoiceOf {
    "CREDIT"
    "DEBIT"
}

let transactionRegex = Regex {
    Anchor.startOfLine
    Capture(kindRegex, as: kindRef)
    OneOrMore(.anyNonNewline)
    kindRef
    Anchor.endOfLine
}

let validTransaction = "CREDIT     109912311421    Payroll   $69.73  CREDIT"
let invalidTransaction = "DEBIT     00522142123    Expense   $5.17  CREDIT"

print(validTransaction.contains(transactionRegex))
// Prints "true"
print(invalidTransaction.contains(transactionRegex))
// Prints "false"
```

Any reference that is used for matching must be captured elsewhere in the `Regex` block. You can use a reference for matching before it is captured; in that case, the reference will not match until it has previously been captured.

To access the captured “transaction kind”, you can use the `kind` reference to subscript a `Regex.Match` instance:

```
if let match = validTransaction.firstMatch(of: transactionRegex) {
    print(match[kindRef])
}
// Prints "CREDIT"
```

To use a `Reference` to capture a transformed value, include a `transform` closure when capturing.

```
struct Transaction {
    var id: UInt64
}
let transactionRef = Reference(Transaction.self)

let transactionIDRegex = Regex {
    Capture(kindRegex, as: kindRef)
    OneOrMore(.whitespace)
    TryCapture(as: transactionRef) {
        OneOrMore(.digit)
    } transform: { str in
        UInt64(str).map(Transaction.init(id:))
    }
    OneOrMore(.anyNonNewline)
    kindRef
    Anchor.endOfLine
}

if let match = validTransaction.firstMatch(of: transactionIDRegex) {
    print(match[transactionRef])
}
// Prints "Transaction(id: 109912311421)"
```

## Topics

### Initializers

init(Capture.Type)

Creates a reference with the specified capture type.

### Instance Properties

var regex: Regex&lt;Capture>

The regular expression represented by this component.

### Type Aliases

typealias RegexOutput

The output type for this regular expression.

## Relationships

### Conforms To

- RegexComponent

## See Also

### Captures

struct Capture

A regex component that saves the matched substring, or a transformed result, for access in a regex match.

struct TryCapture

A regex component that attempts to transform a matched substring, saving the result if successful and backtracking if the transformation fails.

