

- RealityKit
-  MeshBuffer 

Structure

# MeshBuffer

Mesh buffer containing elements of any type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct MeshBuffer
```

## Topics

### Creating a mesh buffer

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init([Element])

Create buffer from an array of elements.

init([Element])

Create buffer from an array of elements.

init([Element])

Create buffer from an array of elements.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

### Inspecting a mesh

let count: Int

The number of elements in the buffer.

var elements: [Element]

Access the buffer as an array. This may create a copy if the data are not already an array.

typealias Element

A type representing the sequence’s elements.

var rate: MeshBuffers.Rate

Rate of the buffer.

### Iterating the elements of a buffer

func makeIterator() -> MeshBuffer&lt;Element>.Iterator

Returns an iterator over the elements of this sequence.

struct Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

func forEach((Element, Element) throws -> Void) rethrows

Iterate over pairs of elements.

func forEach((Element, Element, Element) throws -> Void) rethrows

Iterate over three elements per step.

func forEach((Element, Element, Element, Element) throws -> Void) rethrows

Iterate over four elements per step.

func usingRate(MeshBuffers.Rate) -> MeshBuffer&lt;Element>

New object with updated rate.

### Initializers

init([Element])

Create buffer from an array of elements.

init&lt;S>(S)

Create a buffer from any sequence of elements.

init(elements: [Element], indices: [UInt32])

Create buffer from an array of element values and an array of indices into that value array.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Sequence

## See Also

### Mesh description

protocol MeshBufferContainer

Conforming objects contain a table of mesh buffers.

protocol MeshBufferSemantic

A protocol that holds an identifier value for mesh buffers.

enum MeshBuffers

An object that holds the data for an model entity’s mesh.

struct AnyMeshBuffer

Mesh buffer stored in the container.

struct MeshInstanceCollection

An object that holds a collection of mesh resource instances.

struct MeshModelCollection

An object that holds a collection of mesh models.

struct MeshPartCollection

An object that holds a collection of mesh parts.

