

- RealityKit
-  MeshBuffers 

Enumeration

# MeshBuffers

An object that holds the data for an model entity’s mesh.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum MeshBuffers
```

## Topics

### Structures

struct Identifier

struct Semantic

### Type Aliases

typealias BlendShapeOffsets

typealias JointInfluences

typealias Normals

typealias Positions

typealias Tangents

typealias TextureCoordinates

typealias TriangleIndices

### Type Properties

static let bitangents: MeshBuffers.Semantic&lt;SIMD3&lt;Float>>

static let jointInfluences: MeshBuffers.Semantic&lt;MeshJointInfluence>

static let normals: MeshBuffers.Semantic&lt;SIMD3&lt;Float>>

static let positions: MeshBuffers.Semantic&lt;SIMD3&lt;Float>>

static let tangents: MeshBuffers.Semantic&lt;SIMD3&lt;Float>>

static let textureCoordinates: MeshBuffers.Semantic&lt;SIMD2&lt;Float>>

static let triangleIndices: MeshBuffers.Semantic&lt;UInt32>

### Type Methods

static func blendShapeOffsets(named: String) -> MeshBuffers.Semantic&lt;SIMD3&lt;Float>>

static func custom&lt;Value>(String, type: Value.Type) -> MeshBuffers.Semantic&lt;Value>

### Enumerations

enum ElementType

The data type for each element of the buffer.

enum Rate

Defines how elements in the buffer map to features of the mesh.

## See Also

### Mesh description

struct MeshBuffer

Mesh buffer containing elements of any type.

protocol MeshBufferContainer

Conforming objects contain a table of mesh buffers.

protocol MeshBufferSemantic

A protocol that holds an identifier value for mesh buffers.

struct AnyMeshBuffer

Mesh buffer stored in the container.

struct MeshInstanceCollection

An object that holds a collection of mesh resource instances.

struct MeshModelCollection

An object that holds a collection of mesh models.

struct MeshPartCollection

An object that holds a collection of mesh parts.

