

- RegexBuilder
-  Capture 

Structure

# Capture

A regex component that saves the matched substring, or a transformed result, for access in a regex match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Capture
```

## Overview

Use a `Capture` component to capture one part of a regex to access separately after matching. In the example below, `regex` matches a dollar sign (`"$"`) followed by one or more digits, a period (`"."`), and then two additional digits, as long as that pattern appears at the end of the line. Because the `Capture` block wraps the digits and period, that part of the match is captured separately.

```
let transactions = """
    CREDIT     109912311421    Payroll   $69.73
    CREDIT     105912031123    Travel   $121.54
    DEBIT      107733291022    Refund    $8.42
    """

let regex = Regex {
    "$"
    Capture {
      OneOrMore(.digit)
      "."
      Repeat(.digit, count: 2)
    }
    Anchor.endOfLine
}

// The type of each match's output is `(Substring, Substring)`.
for match in transactions.matches(of: regex) {
    print("Transaction amount: \(match.1)")
}
// Prints "Transaction amount: 69.73"
// Prints "Transaction amount: 121.54"
// Prints "Transaction amount: 8.42"
```

Each `Capture` block increases the number of components in the regex’s output type. In the example above, the capture type of each match is `(Substring, Substring)`.

By providing a transform function to the `Capture` block, you can change the type of the captured value from `Substring` to the result of the transform. This example declares `doubleValueRegex`, which converts the captured amount to a `Double`:

```
let doubleValueRegex = Regex {
    "$"
    Capture {
        OneOrMore(.digit)
        "."
        Repeat(.digit, count: 2)
    } transform: { Double($0)! }
    Anchor.endOfLine
}

// The type of each match's output is `(Substring, Double)`.
for match in transactions.matches(of: doubleValueRegex) {
    if match.1 >= 100.0 {
        print("Large amount: \(match.1)")
    }
}
// Prints "Large amount: 121.54"
```

Throwing an error from a `transform` closure aborts matching and propagates the error out to the caller. If you instead want to use a failable transformation, where a `nil` result participates in matching, use TryCapture instead of `Capture`.

## Topics

### Initializers

init&lt;W, C1>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5>(some RegexComponent)

Creates a capture for the given component.

init&lt;W>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(() -> some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3>(some RegexComponent)

Creates a capture for the given component.

init&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3>(some RegexComponent, as: Reference&lt;W>)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, NewCapture>(some RegexComponent, as: Reference&lt;NewCapture>, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(() -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, NewCapture>(some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5, C6>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, C5>(as: Reference&lt;W>, () -> some RegexComponent)

Creates a capture for the given component using the specified reference.

init&lt;W, C1, C2, C3, C4, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

init&lt;W, C1, C2, C3, C4, C5, C6, NewCapture>(as: Reference&lt;NewCapture>, () -> some RegexComponent, transform: (W) throws -> NewCapture)

Creates a capture for the given component using the specified reference, transforming with the given closure.

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

struct TryCapture

A regex component that attempts to transform a matched substring, saving the result if successful and backtracking if the transformation fails.

struct Reference

A reference to a captured portion of a regular expression.

