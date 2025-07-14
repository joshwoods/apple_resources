

- Model I/O
-  MDLSubmesh 

Class

# MDLSubmesh

A container for index buffer data and material information to be used in rendering all or part of a 3D object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLSubmesh
```

## Overview

Submeshes are contained in MDLMesh objects, which provide vertex buffer data that a submesh’s index data refers to. Together, the vertex and index data describe the geometric form of a portion of the mesh, and the submesh’s material property determines its intended surface appearance for rendering.

## Topics

### Creating a Submesh

init(indexBuffer: any MDLMeshBuffer, indexCount: Int, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType, material: MDLMaterial?)

Initializes a submesh with an index buffer and the specified properties.

init(name: String, indexBuffer: any MDLMeshBuffer, indexCount: Int, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType, material: MDLMaterial?)

Initializes a named submesh with an index buffer and the specified properties.

init(name: String, indexBuffer: any MDLMeshBuffer, indexCount: Int, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType, material: MDLMaterial?, topology: MDLSubmeshTopology?)

Initializes a named submesh with a specific topology.

init?(mdlSubmesh: MDLSubmesh, indexType: MDLIndexBitDepth, geometryType: MDLGeometryType)

Initializes a submesh by copying or converting another submesh.

### Working with a Submesh’s Index Buffer

var indexBuffer: any MDLMeshBuffer

An object that provides index data for the submesh.

var indexCount: Int

The number of indices in the submesh’s index buffer.

var indexType: MDLIndexBitDepth

The data type for each element in the submesh’s index buffer.

var geometryType: MDLGeometryType

The type of geometric primitives described by the submesh’s index buffer.

var topology: MDLSubmeshTopology?

A description of how the non-uniform layout of the submesh’s index buffer defines the shape of the mesh.

func indexBuffer(asIndexType: MDLIndexBitDepth) -> any MDLMeshBuffer

### Associating Materials with a Submesh

var material: MDLMaterial?

An object that describes the intended surface appearance of the submesh for rendering.

### Identifying a Submesh

var name: String

A descriptive name for the submesh.

### Constants

enum MDLIndexBitDepth

Options for the size of integer data in a submesh’s index buffer, used by the indexType property.

enum MDLGeometryType

Types of geometric primitives for rendering a submesh, used by the geometryType property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### 3D Asset Basics

class MDLAsset

An indexed container for 3D objects and associated information, such as transform hierarchies, meshes, cameras, and lights.

class MDLObject

The base class for objects that are part of a 3D asset, including meshes, cameras, and lights.

class MDLTransform

A description of the local coordinate space transformations for a 3D object.

class MDLMesh

A container for vertex buffer data to be used in rendering a 3D object.

class MDLSubmeshTopology

A description of how a submesh’s index buffer data is arranged and how that arrangement should be used to produce the submesh’s intended 3D shape.

protocol MDLNamed

The common interface for Model I/O objects that expose a human-readable name.

