

- RegexBuilder
-  TryCapture 

Structure

# TryCapture

A regex component that attempts to transform a matched substring, saving the result if successful and backtracking if the transformation fails.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct TryCapture
```

## Overview

You use a `TryCapture` component to capture part of a match as a transformed value, when a failure to transform should mean the regex continues matching, backtracking from that point if necessary.

The code below demonstrates using `TryCapture` to include a test that the `Double` value of a capture is over a limit. In the example, `regex` matches a dollar sign (`"$"`) followed by one or more digits, a period (`"."`), and then two additional digits, as long as that pattern appears at the end of the line. The `TryCapture` block wraps the digits and period, capturing that part of the match separately and passing it to its `transform` closure. That closure converts the captured portion of the match, converts it to a `Double`, and only returns a non-`nil` value if it is over the transaction limit.

```
let transactions = """
    CREDIT     109912311421    Payroll   $69.73
    CREDIT     105912031123    Travel   $121.54
    DEBIT      107733291022    Refund    $8.42
    """
let transactionLimit = 100.0

let regex = Regex {
    "$"
    TryCapture {
        OneOrMore(.digit)
        "."
        Repeat(.digit, count: 2)
    } transform: { str -> Double? in
        let value = Double(str)!
        if value > transactionLimit {
            return value
        }
        return nil
    }
    Anchor.endOfLine
}
```

When the `TryCapture` block’s `transform` closure processes the three different amounts in the list of transactions, it only returns a non-`nil` value for the \$121.54 transaction. Even though the capture returns an optional `Double` value, the captured value is non-optional.

```
// The type of each match's output is `(Substring, Double)`.
for match in transactions.matches(of: regex) {
    print("Transaction amount: \(match.1)")
}
// Prints "Transaction amount: 121.54"
```

Throwing an error from a `transform` closure aborts matching and propagates the error out to the caller. If you want to capture the `nil` results of a failable transformation, instead of continuing a search, use Capture instead of `TryCapture`.

## Topics

### Initializers

init&lt;W, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, C1, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component, attempting to transform with the given closure.

init&lt;W, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

init&lt;W, C1, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture?)

Creates a capture for the given component using the specified reference, attempting to transform with the given closure.

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

### Captures

struct Capture

A regex component that saves the matched substring, or a transformed result, for access in a regex match.

struct Reference

A reference to a captured portion of a regular expression.

