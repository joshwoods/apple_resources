

- SwiftUI
- SpatialEventCollection
-  SpatialEventCollection.Iterator 

Structure

# SpatialEventCollection.Iterator

An iterator over all events in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
struct Iterator
```

## Topics

### Getting the next event

func next() -> SpatialEventCollection.Event?

The next `Event` in the sequence, if one exists.

## Relationships

### Conforms To

- IteratorProtocol

## See Also

### Iterating over events in the collection

func makeIterator() -> SpatialEventCollection.Iterator

Makes an iterator over all events in the collection.

