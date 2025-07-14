

- Swift
-  RegexWordBoundaryKind 

Structure

# RegexWordBoundaryKind

A word boundary algorithm to use during regex matching.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct RegexWordBoundaryKind
```

## Overview

See wordBoundaryKind(_:) for information about specifying the word boundary kind for all or part of a regex.

## Topics

### Operators

static func == (RegexWordBoundaryKind, RegexWordBoundaryKind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var `default`: RegexWordBoundaryKind

A word boundary algorithm that implements the “default word boundary” Unicode recommendation.

static var simple: RegexWordBoundaryKind

A word boundary algorithm that implements the “simple word boundary” Unicode recommendation.

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

struct RegexRepetitionBehavior

Specifies how much to attempt to match when using a quantifier.

struct RegexSemanticLevel

A semantic level to use during regex matching.

struct AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

protocol RegexComponent

A type that represents a regular expression.

protocol CustomConsumingRegexComponent

