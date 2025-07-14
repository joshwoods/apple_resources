

- RealityKit
- Models and meshes
- MeshResource.Part
-  MeshBufferContainer Implementations 

API Collection

# MeshBufferContainer Implementations

## Topics

### Instance Properties

var bitangents: MeshBuffers.Tangents?

Buffer of bitangents, if any.

var blendShapeNames: [String]

An array of blendShape names that exist in MeshBufferContainer

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

