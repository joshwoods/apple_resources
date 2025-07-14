

- RealityKit
- LowLevelMesh
-  LowLevelMesh.PartsCollection 

Structure

# LowLevelMesh.PartsCollection

An object that holds a mutable collection low-level mesh parts.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PartsCollection
```

## Topics

### Updating collection contents

func append(LowLevelMesh.PartsCollection.Element)

Adds an element to the end of the collection.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

func replaceAll&lt;S>(S)

Replaces all mesh parts in this collection with those from the new sequence.

func removeAll()

Removes all mesh parts from this collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Updatable meshes

Creating a spatial drawing app with RealityKit

Use low-level mesh and texture APIs to achieve fast updates to a person’s brush strokes by integrating RealityKit with ARKit and SwiftUI.

Creating a plane with low-level mesh

Create a low-level mesh and set its vertex positions and normals to form a plane.

class LowLevelMesh

A container for vertex data that you can use to create and update meshes using your own format.

struct Descriptor

An object that describes the data format and layout of the buffers in a low-level mesh.

struct Part

An object that describes a range of primitives to display, and their material index.

struct Layout

An object that describes a set of attributes that share a buffer index, offset, and stride.

struct Attribute

An object that determines how to store vertex attribute data in memory and map it to RealityKit shader attributes.

enum VertexSemantic

Designates the intended usage of a vertex attribute.

