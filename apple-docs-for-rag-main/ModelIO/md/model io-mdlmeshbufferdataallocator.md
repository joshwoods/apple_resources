

- Model I/O
-  MDLMeshBufferDataAllocator 

Class

# MDLMeshBufferDataAllocator

A basic allocator implementation that allocates from main memory using data objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMeshBufferDataAllocator
```

## Overview

Model I/O uses this allocator by default if you do not specify an allocator when loading, creating, or modifying objects that require mesh buffer storage (for example, when loading an asset with the init(url:vertexDescriptor:bufferAllocator:) initializer). Use this allocator only if sharing mesh buffer memory with GPU-based renderers is not a concern. To minimize data copying when rendering with Metal or OpenGL, use the MTKMeshBufferAllocator or GLKMeshBufferAllocator class instead.This class declares no methods or properties of its own. For the key functionality of all mesh buffer allocator objects, see MDLMeshBufferAllocator.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLMeshBufferAllocator
- NSObjectProtocol

## See Also

### Managing Mesh Data

protocol MDLMeshBuffer

The general interface for managing storage of vertex and index data used in loading, processing, and rendering meshes.

protocol MDLMeshBufferAllocator

The general interface for managing allocation of data buffers to be used in loading, processing, and rendering meshes.

class MDLMeshBufferData

A memory buffer that stores vertex or index data for a Model I/O mesh.

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

