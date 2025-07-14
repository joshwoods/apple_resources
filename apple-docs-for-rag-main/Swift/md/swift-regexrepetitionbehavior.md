

- Swift
-  RegexRepetitionBehavior 

Structure

# RegexRepetitionBehavior

Specifies how much to attempt to match when using a quantifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct RegexRepetitionBehavior
```

## Overview

See repetitionBehavior(_:) for more about specifying the default matching behavior for all or part of a regex.

## Topics

### Operators

static func == (RegexRepetitionBehavior, RegexRepetitionBehavior) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var eager: RegexRepetitionBehavior

Match as much of the input string as possible, backtracking when necessary.

static var possessive: RegexRepetitionBehavior

Match as much of the input string as possible, performing no backtracking.

static var reluctant: RegexRepetitionBehavior

Match as little of the input string as possible, expanding the matched region as necessary to complete a match.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Regular Expressions

struct Regex

A regular expression.

struct RegexSemanticLevel

A semantic level to use during regex matching.

struct RegexWordBoundaryKind

A word boundary algorithm to use during regex matching.

struct AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

protocol RegexComponent

A type that represents a regular expression.

protocol CustomConsumingRegexComponent

