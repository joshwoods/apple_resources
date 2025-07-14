

- Swift
- Sequence
-  Iterator 

Associated Type

# Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
associatedtype Iterator : IteratorProtocol
```

**Required**

## See Also

### Creating an Iterator

func makeIterator() -> Self.Iterator

Returns an iterator over the elements of this sequence.

**Required** Default implementations provided.

associatedtype Element

A type representing the sequence’s elements.

**Required**

