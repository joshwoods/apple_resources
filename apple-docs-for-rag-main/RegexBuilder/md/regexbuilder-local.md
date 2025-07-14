

- RegexBuilder
-  Local 

Structure

# Local

A regex component that represents an atomic group.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Local
```

## Overview

An atomic group opens a local backtracking scope which, upon successful exit, discards any remaining backtracking points from within the scope.

## Topics

### Initializers

init(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5>(some RegexComponent)

Creates an atomic group with the given regex component.

init(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(() -> some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2>(some RegexComponent)

Creates an atomic group with the given regex component.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent)

Creates an atomic group with the given regex component.

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

### Quantifiers

struct One

A regex component that matches exactly one occurrence of its underlying component.

struct Optionally

A regex component that matches zero or one occurrences of its underlying component.

struct ZeroOrMore

A regex component that matches zero or more occurrences of its underlying component.

struct OneOrMore

A regex component that matches one or more occurrences of its underlying component.

struct Repeat

A regex component that matches a selectable number of occurrences of its underlying component.

