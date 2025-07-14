

- Swift
- Dictionary
- Dictionary.Keys
-  Dictionary.Keys.Iterator 

Structure

# Dictionary.Keys.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Key` conforms to `Hashable`.

## Overview

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

## Topics

### Instance Methods

func next() -> Key?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol
- Sendable

  Conforms when `Key` conforms to `Hashable`, `Key` conforms to `Sendable`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, and `Value` conforms to `Sendable`.

