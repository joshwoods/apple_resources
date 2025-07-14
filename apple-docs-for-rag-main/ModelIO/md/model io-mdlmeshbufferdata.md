

- Model I/O
-  MDLMeshBufferData 

Class

# MDLMeshBufferData

A memory buffer that stores vertex or index data for a Model I/O mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMeshBufferData
```

## Overview

This class is the simplest concrete implementation of the MDLMeshBuffer protocol—use this class when you need only a single data store for loading or processing mesh data. To share mesh data for other uses, use another concrete implementation of the MDLMeshBuffer protocol—for example, the MTKMeshBuffer class shares mesh data with Metal buffers, ensuring that data is copied a minimal number of times between loading, processing, and rendering.If you do not specify a MDLMeshBufferAllocator object for loading meshes from a file with the MDLAsset class or generating meshes with the MDLMesh class, Model I/O uses MDLMeshBufferData objects to store mesh data.

## Topics

### Creating a Buffer

init(type: MDLMeshBufferType, data: Data?)

Initializes a buffer containing the specified data.

init(type: MDLMeshBufferType, length: Int)

Initializes a buffer of the specified length.

### Accessing a Buffer’s Data

var data: Data

The underlying data storage for the mesh buffer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLMeshBuffer
- NSCopying
- NSObjectProtocol

## See Also

### Managing Mesh Data

protocol MDLMeshBuffer

The general interface for managing storage of vertex and index data used in loading, processing, and rendering meshes.

protocol MDLMeshBufferAllocator

The general interface for managing allocation of data buffers to be used in loading, processing, and rendering meshes.

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

