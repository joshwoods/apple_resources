

- Swift
- String
-  String.Iterator 

Structure

# String.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

## Overview

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

## Topics

### Instance Methods

func next() -> Character?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol
- Sendable

## See Also

### Related String Types

struct Substring

A slice of a string.

protocol StringProtocol

A type that can represent a string as a collection of characters.

struct Index

A position of a character or code unit in a string.

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct Encoding

