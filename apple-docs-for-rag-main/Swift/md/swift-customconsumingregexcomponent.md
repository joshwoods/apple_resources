

- Swift
-  CustomConsumingRegexComponent 

Protocol

# CustomConsumingRegexComponent

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CustomConsumingRegexComponent : RegexComponent
```

## Topics

### Instance Methods

func consuming(String, startingAt: String.Index, in: Range&lt;String.Index>) throws -> (upperBound: String.Index, output: Self.RegexOutput)?

Process the input string within the specified bounds, beginning at the given index, and return the end position (upper bound) of the match and the produced output.

**Required**

## Relationships

### Inherits From

- RegexComponent

## See Also

### Regular Expressions

struct Regex

A regular expression.

struct RegexRepetitionBehavior

Specifies how much to attempt to match when using a quantifier.

struct RegexSemanticLevel

A semantic level to use during regex matching.

struct RegexWordBoundaryKind

A word boundary algorithm to use during regex matching.

struct AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

protocol RegexComponent

A type that represents a regular expression.

