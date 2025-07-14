

- RealityKit
-  MeshBufferContainer 

Protocol

# MeshBufferContainer

Conforming objects contain a table of mesh buffers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol MeshBufferContainer
```

## Topics

### Instance Properties

var bitangents: MeshBuffers.Tangents?

Buffer of bitangents, if any.

var blendShapeNames: [String]

An array of blendShape names that exist in MeshBufferContainer

var buffers: [MeshBuffers.Identifier : AnyMeshBuffer]

Descriptors for the buffers.

**Required**

var normals: MeshBuffers.Normals?

Buffer of normals, if any.

var positions: MeshBuffers.Positions

Positions of all the points.

var tangents: MeshBuffers.Tangents?

Buffer of tangents, if any.

var textureCoordinates: MeshBuffers.TextureCoordinates?

Buffer of texture coordinates, if any.

### Instance Methods

func blendShapeOffsets(named: String) -> MeshBuffers.BlendShapeOffsets?

func setBlendShapeOffsets(named: String, buffer: MeshBuffers.BlendShapeOffsets?)

### Subscripts

subscript&lt;S>(S) -> MeshBuffer&lt;S.Element>?

The buffer for a given semantic. There can only be one buffer for any given ID.

**Required**

## Relationships

### Conforming Types

- MeshDescriptor
- MeshResource.Part

## See Also

### Mesh description

struct MeshBuffer

Mesh buffer containing elements of any type.

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

