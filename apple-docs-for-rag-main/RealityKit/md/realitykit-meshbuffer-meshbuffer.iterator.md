

- RealityKit
- MeshBuffer
-  MeshBuffer.Iterator 

Structure

# MeshBuffer.Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() -> Element?

Advances to the next element and returns it, or `nil` if no next element exists.

## Relationships

### Conforms To

- IteratorProtocol

## See Also

### Iterating the elements of a buffer

func makeIterator() -> MeshBuffer&lt;Element>.Iterator

Returns an iterator over the elements of this sequence.

func forEach((Element, Element) throws -> Void) rethrows

Iterate over pairs of elements.

func forEach((Element, Element, Element) throws -> Void) rethrows

Iterate over three elements per step.

func forEach((Element, Element, Element, Element) throws -> Void) rethrows

Iterate over four elements per step.

func usingRate(MeshBuffers.Rate) -> MeshBuffer&lt;Element>

New object with updated rate.

