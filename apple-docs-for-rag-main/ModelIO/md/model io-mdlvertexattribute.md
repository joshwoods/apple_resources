

- Model I/O
-  MDLVertexAttribute 

Class

# MDLVertexAttribute

A description of the format of per-vertex data for a single vertex attribute in a mesh object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLVertexAttribute
```

## Overview

The vertex buffers of a MDLMesh object store vertex attributes—such as vertex position, surface normal vector, or texture coordinates—that define its 3D shape and other data for use in rendering. Attribute information describes the structure and layout of that data. A collection of vertex attribute objects and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

## Topics

### Creating a Vertex Attribute

init(name: String, format: MDLVertexFormat, offset: Int, bufferIndex: Int)

Initializes a vertex attribute object with the specified property values.

### Inspecting a Vertex Attribute

var name: String

An identifier for the semantic use of the vertex attribute.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

var offset: Int

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

var bufferIndex: Int

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

var initializationValue: vector_float4

The default value for vertex data for this attribute.

### Constants

Vertex Attributes

Names that identify semantic uses for vertex attribute data, used by the name property.

enum MDLVertexFormat

Descriptions of the data size and layout for a vertex attribute, used by the format property.

### Instance Properties

var time: TimeInterval

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

class MDLVertexAttributeData

An object that provides convenience access to vertex data for a specific vertex attribute of a mesh.

class MDLVertexBufferLayout

A MDLVertexBufferLayout object describes layout information for a vertex buffer in a MDLMesh object. A collection of vertex layer objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

class MDLVertexDescriptor

A description of the structure, format, and layout for vertex data buffers associated with a mesh.

