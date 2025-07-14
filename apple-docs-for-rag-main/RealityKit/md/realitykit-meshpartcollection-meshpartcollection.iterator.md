

- RealityKit
- MeshPartCollection
-  MeshPartCollection.Iterator 

Structure

# MeshPartCollection.Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() -> MeshResource.Part?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol

