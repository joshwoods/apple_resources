

- RealityKit
- QueryResult
-  QueryResult.Iterator 

Structure

# QueryResult.Iterator

The type of iterator used for entity query results.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Iterator
```

## Topics

### Advancing the iterator

func next() -> Element?

Advances to the next entity and returns it.

## Relationships

### Conforms To

- IteratorProtocol

## See Also

### Creating an iterator

func makeIterator() -> QueryResult&lt;Element>.Iterator

Returns an iterator for the contained entities.

