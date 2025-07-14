

- Model I/O
-  MDLMeshBufferZoneDefault 

Class

# MDLMeshBufferZoneDefault

A standard implementation of the MDLMeshBufferZone protocol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLMeshBufferZoneDefault
```

## Overview

Model I/O uses zones to ensure that related allocations—such as the multiple vertex and index buffers associated with a MDLMesh object—use contiguous blocks of memory for optimal performance. When working with a MDLMeshBufferAllocator object that does not implement its own zone management, Model I/O uses this zone class.This class declares no methods or properties of its own. For the key functionality of all mesh buffer zone objects, see MDLMeshBufferZone.

## Topics

### Instance Properties

var allocator: any MDLMeshBufferAllocator

var capacity: Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLMeshBufferZone
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

class MDLVertexAttribute

A description of the format of per-vertex data for a single vertex attribute in a mesh object.

class MDLVertexAttributeData

An object that provides convenience access to vertex data for a specific vertex attribute of a mesh.

class MDLVertexBufferLayout

A MDLVertexBufferLayout object describes layout information for a vertex buffer in a MDLMesh object. A collection of vertex layer objects, vertex attribute objects, and additional information forms a MDLVertexDescriptor object, which completely describes the layout of vertex buffers for a mesh.

class MDLVertexDescriptor

A description of the structure, format, and layout for vertex data buffers associated with a mesh.

