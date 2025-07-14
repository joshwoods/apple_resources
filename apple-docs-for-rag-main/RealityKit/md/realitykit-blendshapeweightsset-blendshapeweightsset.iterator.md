

- RealityKit
- BlendShapeWeightsSet
-  BlendShapeWeightsSet.Iterator 

Structure

# BlendShapeWeightsSet.Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() -> BlendShapeWeightsSet.Element?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol

