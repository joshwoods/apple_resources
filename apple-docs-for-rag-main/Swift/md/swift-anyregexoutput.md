

- Swift
-  AnyRegexOutput 

Structure

# AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AnyRegexOutput
```

## Overview

When you find a match using regular expression that has `AnyRegexOutput` as its output type, you can find information about matches by iterating

## Topics

### Initializers

init&lt;Output>(Regex&lt;Output>.Match)

Creates a dynamic regular expression match output from an existing match.

### Instance Methods

func extractValues&lt;Output>(as: Output.Type) -> Output?

Returns strongly-typed match output by converting this type-erased output to the specified type, if possible.

### Subscripts

subscript(String) -> AnyRegexOutput.Element?

Accesses the capture with the specified name, if a capture with that name exists.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- RandomAccessCollection
- Sequence

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

protocol RegexComponent

A type that represents a regular expression.

protocol CustomConsumingRegexComponent

