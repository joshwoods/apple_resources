

- Model I/O
-  MDLMeshBufferMap 

Class

# MDLMeshBufferMap

An object that manages access to a memory buffer used for the data storage of a Model I/O mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMeshBufferMap
```

## Overview

Typically, you do not create MDLMeshBufferMap objects directly. Instead, you use classes supporting the MDLMeshBuffer protocol to manage mesh buffer memory shared with a rendering technology—for example, the MTKMeshBuffer class for rendering with Metal. A mesh buffer object vends a MDLMeshBufferMap objects when you use the map() method to gain temporary access to the shared memory.

Important

When you use a mesh buffer’s map() method, the buffer remains mapped for as long as that MDLMeshBufferMap object exists. Mapping a buffer may impose restrictions on a system. For example, a buffer in shared GPU memory may be unavailable for rendering while mapped, causing draw calls that use the buffer to fail until the corresponding MDLMeshBufferMap object is deallocated.

## Topics

### Creating a Buffer Map

init(bytes: UnsafeMutableRawPointer, deallocator: (() -> Void)?)

Initializes a buffer map object to manage access to the specified memory.

### Accessing Buffer Data

var bytes: UnsafeMutableRawPointer

A pointer to the mutable memory managed by the buffer map.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing Mesh Data

protocol MDLMeshBuffer

The general interface for managing storage of vertex and index data used in loading, processing, and rendering meshes.

protocol MDLMeshBufferAllocator

The general interface for managing allocation of data buffers to be used in loading, processing, and rendering meshes.

class MDLMeshBufferData

A memory buffer that stores vertex or index data for a Model I/O mesh.

class MDLMeshBufferDataAllocator

A basic allocator implementation that allocates from main memory using data objects.

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

