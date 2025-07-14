

- Model I/O
-  MDLMeshBuffer 

Protocol

# MDLMeshBuffer

The general interface for managing storage of vertex and index data used in loading, processing, and rendering meshes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLMeshBuffer : NSCopying, NSObjectProtocol
```

## Overview

Model I/O creates buffers using an allocator that you specify when loading mesh data from a file with the MDLAsset class or generating meshes with the MDLMesh class. You can also create buffers using an allocator method such as newBuffer(with:type:). The allocator you choose determines the concrete class of a mesh buffer and thus its storage mechanism—for example, the MetalKit MTKMeshBufferAllocator class allocates MTKMeshBuffer objects, which share storage with Metal buffers for use in rendering.

## Topics

### Working with Data in a Buffer

func fill(Data, offset: Int)

Writes the specified data into the buffer.

**Required**

func map() -> MDLMeshBufferMap

Provides direct, read-only access to the buffer’s contents.

**Required**

var length: Int

The data size of the buffer, in bytes.

**Required**

### Inspecting a Buffer

var allocator: any MDLMeshBufferAllocator

The allocator object that created the buffer.

**Required**

var zone: any MDLMeshBufferZone

The memory pool from which the buffer was created.

**Required**

var type: MDLMeshBufferType

The type of data contained in a buffer.

**Required**

### Constants

enum MDLMeshBufferType

Options for the content of a mesh buffer, used by the type property and by MDLMeshBufferAllocator methods for creating buffers.

## Relationships

### Inherits From

- NSCopying
- NSObjectProtocol

### Conforming Types

- MDLMeshBufferData

## See Also

### Managing Mesh Data

protocol MDLMeshBufferAllocator

The general interface for managing allocation of data buffers to be used in loading, processing, and rendering meshes.

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

