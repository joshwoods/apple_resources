

- Model I/O
-  MDLMeshBufferZone 

Protocol

# MDLMeshBufferZone

The general interface for logical pools of memory used in allocation of related mesh data buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLMeshBufferZone : NSObjectProtocol
```

## Overview

The concrete type of a zone is often private—you obtain zones by creating them from a MDLMeshBufferAllocator object, then use zones with allocator methods such as newBuffer(from:data:type:) when you need to ensure that related buffers are allocated together.

## Topics

### Inspecting a Zone

var allocator: any MDLMeshBufferAllocator

The allocator object that created the zone.

**Required**

var capacity: Int

The data capacity of the zone, in bytes.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MDLMeshBufferZoneDefault

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

