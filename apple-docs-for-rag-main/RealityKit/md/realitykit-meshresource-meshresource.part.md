

- RealityKit
- MeshResource
-  MeshResource.Part 

Structure

# MeshResource.Part

A part of a model consisting of a single material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Part
```

## Topics

### Initializers

init(id: String, materialIndex: Int)

Create a new part.

### Instance Properties

var buffers: [MeshBuffers.Identifier : AnyMeshBuffer]

Descriptors for the buffers.

var id: String

The stable identity of the entity associated with this instance.

var jointInfluences: MeshResource.JointInfluences?

A buffer of vertex-joint influences which defines how the mesh deforms in response to the skeleton that it is bound to. Each vertex may be influenced by one or more joints defined by the skeleton.

var materialIndex: Int

Material index for the part.

var skeletonID: String?

Identifier of the skeleton that this mesh part is bound to (if it is skinned).

var triangleIndices: MeshBuffers.TriangleIndices?

Index buffer for triangles.

### Subscripts

subscript&lt;S>(S) -> MeshBuffer&lt;S.Element>?

The buffer for a given semantic. There can only be one buffer for any given ID.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

MeshBufferContainer Implementations

## Relationships

### Conforms To

- Identifiable
- MeshBufferContainer

## See Also

### Mesh resource data

struct Contents

Value of the contents of the resource.

struct Instance

An object that transforms a model to a location.

struct Model

A model consists of a list of parts.

