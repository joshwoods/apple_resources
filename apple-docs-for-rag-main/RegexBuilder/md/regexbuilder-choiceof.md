

- RegexBuilder
-  ChoiceOf 

Structure

# ChoiceOf

A regex component that chooses exactly one of its constituent regex components when matching.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct ChoiceOf
```

## Overview

You can use `ChoiceOf` to provide a group of regex components, each of which can be exclusively matched. In this example, `regex` successfully matches either a `"CREDIT"` or `"DEBIT"` substring:

```
let regex = Regex {
    ChoiceOf {
        "CREDIT"
        "DEBIT"
    }
}
let match = try regex.prefixMatch(in: "DEBIT    04032020    Payroll $69.73")
print(match?.0 as Any)
// Prints "DEBIT"
```

## Topics

### Initializers

init(() -> ChoiceOf&lt;Output>)

Creates a regex component that chooses exactly one of the regex components provided by the builder closure.

### Instance Properties

var regex: Regex&lt;Output>

The regular expression represented by this component.

### Type Aliases

typealias RegexOutput

The output type for this regular expression.

## Relationships

### Conforms To

- Copyable

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- RegexComponent

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

## See Also

### Components

struct CharacterClass

A class of characters that match in a regex.

struct Anchor

A regex component that matches a specific condition at a particular position in an input string.

struct Lookahead

A regex component that allows a match to continue only if its contents match at the given location.

struct NegativeLookahead

A regex component that allows a match to continue only if its contents do not match at the given location.

