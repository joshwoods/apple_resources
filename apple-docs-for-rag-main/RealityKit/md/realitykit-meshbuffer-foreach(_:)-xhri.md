

- RealityKit
- MeshBuffer
-  forEach(\_:) 

Instance Method

# forEach(\_:)

Iterate over four elements per step.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func forEach(_ body: (Element, Element, Element, Element) throws -> Void) rethrows
```

## See Also

### Iterating the elements of a buffer

func makeIterator() -> MeshBuffer&lt;Element>.Iterator

Returns an iterator over the elements of this sequence.

struct Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

func forEach((Element, Element) throws -> Void) rethrows

Iterate over pairs of elements.

func forEach((Element, Element, Element) throws -> Void) rethrows

Iterate over three elements per step.

func usingRate(MeshBuffers.Rate) -> MeshBuffer&lt;Element>

New object with updated rate.

