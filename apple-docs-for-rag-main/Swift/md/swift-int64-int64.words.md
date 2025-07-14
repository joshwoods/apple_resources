

- Swift
- Int64
-  Int64.Words 

Structure

# Int64.Words

A type that represents the words of this integer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Words
```

## Topics

### Initializers

init(Int64)

### Instance Properties

var count: Int

The number of elements in the collection.

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var indices: Int64.Words.Indices

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: Int

The position of the first element in a nonempty collection.

### Instance Methods

func index(after: Int) -> Int

Returns the position immediately after the given index.

func index(before: Int) -> Int

Returns the position immediately before the given index.

### Subscripts

subscript(Int) -> UInt

Accesses the element at the specified position.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- BitwiseCopyable
- Collection
- Copyable
- RandomAccessCollection
- Sendable
- Sequence

