

- Foundation
-  Data 

Structure

# Data

A byte buffer in memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Data
```

## Mentioned in 

Processing URL session data task results with Combine

Encoding and Decoding Custom Types

## Overview

The Data value type allows simple byte buffers to take on the behavior of Foundation objects. You can create empty or pre-populated buffers from a variety of sources and later add or remove bytes. You can filter and sort the content, or compare against other buffers. You can manipulate subranges of bytes and iterate over some or all of them.

Data bridges to the NSData class and its mutable subclass, NSMutableData. You can use these interchangeably in code that interacts with Objective-C APIs.

## Topics

### Creating Empty Data

init()

Creates an empty data buffer.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

func resetBytes(in: Range&lt;Data.Index>)

Sets a region of the data buffer to `0`.

### Creating Populated Data

init()

Creates an empty data buffer.

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

init&lt;SourceType>(buffer: UnsafeBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a buffer pointer.

init&lt;SourceType>(buffer: UnsafeMutableBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a mutable buffer pointer.

init(bytes: UnsafeRawPointer, count: Int)

Creates data with copied memory content.

init(bytesNoCopy: UnsafeMutableRawPointer, count: Int, deallocator: Data.Deallocator)

Creates a data buffer with memory content without copying the bytes.

init(capacity: Int)

Creates an empty data buffer of a specified size.

init(count: Int)

Creates a new data buffer with the specified count of zeroed bytes.

### Creating Data from Raw Memory

init(bytes: UnsafeRawPointer, count: Int)

Creates data with copied memory content.

init&lt;SourceType>(buffer: UnsafeBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a buffer pointer.

init&lt;SourceType>(buffer: UnsafeMutableBufferPointer&lt;SourceType>)

Creates a data buffer with copied memory content using a mutable buffer pointer.

init(bytesNoCopy: UnsafeMutableRawPointer, count: Int, deallocator: Data.Deallocator)

Creates a data buffer with memory content without copying the bytes.

enum Deallocator

A deallocator you use to customize how the backing store is deallocated for data created with the no-copy initializer.

### Reading and Writing Data

func write(to: URL, options: Data.WritingOptions) throws

Writes the contents of the data buffer to a location.

typealias ReadingOptions

Options to control the reading of data from a URL.

typealias WritingOptions

Options to control the writing of data to a URL.

### Base-64 Encoding

func base64EncodedData(options: Data.Base64EncodingOptions) -> Data

Returns Base-64 encoded data.

func base64EncodedString(options: Data.Base64EncodingOptions) -> String

Returns a Base-64 encoded string.

typealias Base64DecodingOptions

Options to use when decoding data.

typealias Base64EncodingOptions

Options to use when encoding data.

### Counting Bytes

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

### Accessing Bytes

subscript(Data.Index) -> UInt8

Accesses the byte at the specified index.

### Accessing Underlying Memory

func withUnsafeBytes&lt;ResultType, ContentType>((UnsafePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Accesses the raw bytes in the data’s buffer.

func withUnsafeMutableBytes&lt;ResultType, ContentType>((UnsafeMutablePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Mutates the raw bytes in the data’s buffer.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

Copies the contents of the data to memory.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;Data.Index>)

Copies a subset of the contents of the data to memory.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;Data.Index>?) -> Int

Copies the bytes in a range from the data into a buffer.

### Adding Bytes

func append(Data)

Appends the specified data to the end of this data.

func append&lt;SourceType>(UnsafeBufferPointer&lt;SourceType>)

Append a buffer of bytes to the data.

func append(UnsafePointer&lt;UInt8>, count: Int)

Appends the specified bytes from memory to the end of the data.

func append(contentsOf: [UInt8])

Appends the bytes in the specified array to the end of the data.

### Removing Bytes

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

func removeAll(keepingCapacity: Bool)

Removes all elements from the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

### Replacing a Range of Bytes

func replaceSubrange(Range&lt;Data.Index>, with: Data)

Replaces a region of bytes in the data with new data.

func replaceSubrange&lt;ByteCollection>(Range&lt;Data.Index>, with: ByteCollection)

Replaces a region of bytes in the data with new bytes from a collection.

func replaceSubrange&lt;SourceType>(Range&lt;Data.Index>, with: UnsafeBufferPointer&lt;SourceType>)

Replaces a region of bytes in the data with new bytes from a buffer.

func replaceSubrange(Range&lt;Data.Index>, with: UnsafeRawPointer, count: Int)

Replaces a region of bytes in the data with bytes from memory.

### Finding Bytes

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func range(of: Data, options: Data.SearchOptions, in: Range&lt;Data.Index>?) -> Range&lt;Data.Index>?

Finds the range of the specified data as a subsequence of this data, if it exists.

typealias SearchOptions

Options that control a data search operation.

### Selecting Bytes

func filter((Self.Element) throws -> Bool) rethrows -> Self

Returns a new collection of the same type containing, in order, the elements of the original collection that satisfy the given predicate.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

### Excluding Bytes

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func advanced(by: Int) -> Data

Returns a new data buffer created by removing the given number of bytes from the front of the original buffer.

### Transforming Data

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

### Iterating Over Bytes

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func makeIterator() -> Data.Iterator

Returns an iterator over the contents of the data.

func enumerateBytes((UnsafeBufferPointer&lt;UInt8>, Data.Index, inout Bool) -> Void)

Enumerates the contents of the data’s buffer.

### Sorting Bytes

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

### Splitting the Buffer

func subdata(in: Range&lt;Data.Index>) -> Data

Returns a new copy of the data in a specified range.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

### Comparing Data

static func == (Data, Data) -> Bool

Returns `true` if the two `Data` arguments are equal.

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the less-than operator (`

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

### Manipulating Indexes

var startIndex: Data.Index

The beginning index into the data.

var endIndex: Data.Index

The end index into the data.

### Describing Data

var description: String

A human-readable description for the data.

var debugDescription: String

A human-readable debug description for the data.

### Using Reference Types

class NSData

A static byte buffer in memory.

class NSMutableData

An object representing a dynamic byte buffer in memory.

### Initializers

init?(base64Encoded: Data, options: Data.Base64DecodingOptions)

init?(base64Encoded: String, options: Data.Base64DecodingOptions)

init(bytes: Array&lt;UInt8>)

init&lt;S>(bytes: S)

init(bytes: ArraySlice&lt;UInt8>)

init(contentsOf: URL, options: Data.ReadingOptions) throws

init(referencing: NSData)

init(repeating: UInt8, count: Int)

### Instance Properties

var count: Int

### Instance Methods

func hash(into: inout Hasher)

The hash value for the data.

func withUnsafeMutableBytes&lt;ResultType>((UnsafeMutableRawBufferPointer) throws -> ResultType) rethrows -> ResultType

### Subscripts

subscript&lt;R>(R) -> Data

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

DataProtocol Implementations

Equatable Implementations

MutableCollection Implementations

MutableDataProtocol Implementations

RandomAccessCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

Transferable Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- CKRecordValueProtocol
- Collection
- ContiguousBytes
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- DataProtocol
- Decodable
- Encodable
- Equatable
- Hashable
- MutableCollection
- MutableDataProtocol
- RandomAccessCollection
- RangeReplaceableCollection
- ReferenceConvertible
- Sendable
- Sequence
- Transferable

## See Also

### Binary Data

protocol DataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous data buffers.

protocol MutableDataProtocol

A protocol that provides consistent data access to the bytes underlying contiguous and noncontiguous mutable data buffers.

protocol ContiguousBytes

A protocol that declares the type offers direct access to the underlying raw bytes in a contiguous manner.

