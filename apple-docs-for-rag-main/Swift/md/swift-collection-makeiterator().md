

- Swift
- Collection
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the elements of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
override func makeIterator() -> Self.Iterator
```

**Required** Default implementation provided.

## Default Implementations

### Sequence Implementations

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

