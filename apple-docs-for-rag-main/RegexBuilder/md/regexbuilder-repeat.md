

- RegexBuilder
-  Repeat 

Structure

# Repeat

A regex component that matches a selectable number of occurrences of its underlying component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Repeat
```

## Topics

### Initializers

init&lt;W, C1, C2, C3, C4, C5, C6>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init(some RangeExpression&lt;Int>, RegexRepetitionBehavior?, () -> some RegexComponent)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent, some RangeExpression&lt;Int>, RegexRepetitionBehavior?)

Creates a regex component that matches the given component repeated a number of times specified by the given range expression.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent, count: Int)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

init&lt;W, C1, C2, C3, C4, C5>(count: Int, () -> some RegexComponent)

Creates a regex component that matches the given component repeated the specified number of times.

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

struct Local

A regex component that represents an atomic group.

