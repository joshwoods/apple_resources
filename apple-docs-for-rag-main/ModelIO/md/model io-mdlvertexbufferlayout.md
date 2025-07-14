

- Model I/O
-  MDLVertexBufferLayout 

Class

# MDLVertexBufferLayout

A MDLVertexBufferLayout object describes layout information for a vertex buffer in a MDLMesh object. A collection of vertex layer objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLVertexBufferLayout
```

## Overview

A collection of vertex layout objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a MDLMesh object.

A mesh may store vertex data in either a structure of arrays model, where data for each vertex attribute (such as vertex position or surface normal) lies in a separate vertex buffer, or in an array of structures model, where multiple vertex attributes share the same buffer.

- In a structure of arrays, the mesh’s vertexBuffers array contains several MDLMeshBuffer objects, and the mesh’s vertexDescriptor object contains a separate MDLVertexBufferLayout object for each buffer.

- In an array of structures, the mesh contains a single vertex buffer, and its descriptor contains a single vertex buffer layout object. To identify which bytes in the buffer refer to which vertices and vertex attributes, use the layout’s stride together with the format and offset properties of the descriptor’s vertex attributes.

Because there is only one stride per buffer:

- If a buffer uses interleaved layout, it can contain attributes of different sizes, and the stride is the sum of their sizes (plus padding).

- If a buffer uses non-interleaved layout (that is, it stores all the data for one attribute, then all the data for another, and so on), each attribute in the buffer must have the same size as the others.

## Topics

### Working with Layout Information

var stride: Int

The stride, in bytes, between data for separate vertices in a vertex buffer.

### Initializers

init(stride: Int)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

class MDLVertexDescriptor

A description of the structure, format, and layout for vertex data buffers associated with a mesh.

