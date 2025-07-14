

- Swift
- Sequence
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the elements of this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> Self.Iterator
```

**Required** Default implementations provided.

## Default Implementations

### Sequence Implementations

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

func makeIterator() -> Self

Returns an iterator over the elements of this sequence.

## See Also

### Creating an Iterator

associatedtype Iterator : IteratorProtocol

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

**Required**

associatedtype Element

A type representing the sequence’s elements.

**Required**

