

- Swift
- Dictionary
-  Dictionary.Keys 

Structure

# Dictionary.Keys

A view of a dictionary’s keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Keys
```

Available when `Key` conforms to `Hashable`.

## Topics

### Operators

static func == (Dictionary&lt;Key, Value>.Keys, Dictionary&lt;Key, Value>.Keys) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var count: Int

The number of keys in the dictionary.

var endIndex: Dictionary&lt;Key, Value>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: Dictionary&lt;Key, Value>.Index

The position of the first element in a nonempty collection.

### Instance Methods

func formIndex(after: inout Dictionary&lt;Key, Value>.Index)

Replaces the given index with its successor.

func index(after: Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Index

Returns the position immediately after the given index.

### Subscripts

subscript(Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Keys.Element

Accesses the element at the specified position.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- CustomDebugStringConvertible

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- CustomStringConvertible

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Equatable
- Sendable

  Conforms when `Key` conforms to `Hashable`, `Key` conforms to `Sendable`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, and `Value` conforms to `Sendable`.

- Sequence

## See Also

### Supporting Types

struct Values

A view of a dictionary’s values.

struct Index

The position of a key-value pair in a dictionary.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

struct Iterator

An iterator over the members of a `Dictionary`.

