

- Model I/O
-  MDLMeshBufferAllocator 

Protocol

# MDLMeshBufferAllocator

The general interface for managing allocation of data buffers to be used in loading, processing, and rendering meshes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLMeshBufferAllocator : NSObjectProtocol
```

## Overview

Classes adopting this protocol provide different ways of handling mesh buffer data. For example, the MTKMeshBufferAllocator class can share mesh data with Metal buffers for use in rendering.

When you load meshes from a file with the MDLAsset class or generate meshes with the MDLMesh class, you must specify an allocator. By choosing an allocator specific to how you use a mesh, you can ensure that vertex and index data for the mesh is copied and transformed a minimal number of times between loading and use.

## Topics

### Allocating Mesh Buffers

func newZone(Int) -> any MDLMeshBufferZone

Creates a zone for related memory allocations.

**Required**

func newZoneForBuffers(withSize: [NSNumber], andType: [NSNumber]) -> any MDLMeshBufferZone

Creates a zone large enough to fit the specified group of allocation sizes.

**Required**

func newBuffer(Int, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer of the specified length.

**Required**

func newBuffer(from: (any MDLMeshBufferZone)?, length: Int, type: MDLMeshBufferType) -> (any MDLMeshBuffer)?

Creates a new buffer of the specified length in the specified zone.

**Required**

func newBuffer(with: Data, type: MDLMeshBufferType) -> any MDLMeshBuffer

Creates a new buffer containing the specified data.

**Required**

func newBuffer(from: (any MDLMeshBufferZone)?, data: Data, type: MDLMeshBufferType) -> (any MDLMeshBuffer)?

Creates a new buffer containing the specified data in the specified zone.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MDLMeshBufferDataAllocator

## See Also

### Managing Mesh Data

protocol MDLMeshBuffer

The general interface for managing storage of vertex and index data used in loading, processing, and rendering meshes.

class MDLMeshBufferData

A memory buffer that stores vertex or index data for a Model I/O mesh.

class MDLMeshBufferDataAllocator

A basic allocator implementation that allocates from main memory using data objects.

class MDLMeshBufferMap

An object that manages access to a memory buffer used for the data storage of a Model I/O mesh.

protocol MDLMeshBufferZone

The general interface for logical pools of memory used in allocation of related mesh data buffers.

class MDLMeshBufferZoneDefault

A standard implementation of the MDLMeshBufferZone protocol.

class MDLVertexAttribute

A description of the format of per-vertex data for a single vertex attribute in a mesh object.

class MDLVertexAttributeData

An object that provides convenience access to vertex data for a specific vertex attribute of a mesh.

class MDLVertexBufferLayout

A MDLVertexBufferLayout object describes layout information for a vertex buffer in a MDLMesh object. A collection of vertex layer objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

class MDLVertexDescriptor

A description of the structure, format, and layout for vertex data buffers associated with a mesh.

