

- RegexBuilder
-  One 

Structure

# One

A regex component that matches exactly one occurrence of its underlying component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct One
```

## Topics

### Initializers

init(some RegexComponent&lt;Output>)

Creates a regex component that matches the given component exactly once.

### Instance Properties

var regex: Regex&lt;Output>

The regular expression represented by this component.

### Type Aliases

typealias RegexOutput

The output type for this regular expression.

## Relationships

### Conforms To

- RegexComponent

## See Also

### Quantifiers

struct Optionally

A regex component that matches zero or one occurrences of its underlying component.

struct ZeroOrMore

A regex component that matches zero or more occurrences of its underlying component.

struct OneOrMore

A regex component that matches one or more occurrences of its underlying component.

struct Repeat

A regex component that matches a selectable number of occurrences of its underlying component.

struct Local

A regex component that represents an atomic group.

