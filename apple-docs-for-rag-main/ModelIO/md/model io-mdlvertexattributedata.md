

- Model I/O
-  MDLVertexAttributeData 

Class

# MDLVertexAttributeData

An object that provides convenience access to vertex data for a specific vertex attribute of a mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLVertexAttributeData
```

## Overview

You retrieve a vertex attribute data object by calling the vertexAttributeData(forAttributeNamed:) method of a MDLMesh object, which is shorthand for looking up the the MDLMeshBuffer object corresponding to the named attribute and using the map() method to gain read-only access to its contents.

## Topics

### Accessing Data for a Vertex Attribute

var dataStart: UnsafeMutableRawPointer

The offset, in bytes, from the start of the data to where vertex attribute information begins.

var stride: Int

The stride, in bytes, between vertex information for consecutive vertices in the data.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

### Instance Properties

var bufferSize: Int

var map: MDLMeshBufferMap

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

class MDLMeshBufferMap

An object that manages access to a memory buffer used for the data storage of a Model I/O mesh.

protocol MDLMeshBufferZone

The general interface for logical pools of memory used in allocation of related mesh data buffers.

class MDLMeshBufferZoneDefault

A standard implementation of the MDLMeshBufferZone protocol.

class MDLVertexAttribute

A description of the format of per-vertex data for a single vertex attribute in a mesh object.

class MDLVertexBufferLayout

A MDLVertexBufferLayout object describes layout information for a vertex buffer in a MDLMesh object. A collection of vertex layer objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

class MDLVertexDescriptor

A description of the structure, format, and layout for vertex data buffers associated with a mesh.

