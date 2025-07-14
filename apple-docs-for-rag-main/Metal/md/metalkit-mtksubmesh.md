

- MetalKit
-  MTKSubmesh 

Class

# MTKSubmesh

A container for the index data of a Model I/O submesh, suitable for use in a Metal app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MTKSubmesh
```

## Overview

The MTKSubmesh class provides a container for a segment of mesh data that can be rendered in a single draw call. A submesh can only be initialized as part of a MTKMesh object. Each submesh contains an index buffer with which the parent’s mesh data can be rendered. Actual submesh vertex data resides in the submesh’s parent mesh. For more information on Model I/O submeshes, see MDLSubmesh.

## Topics

### Parent Mesh

var mesh: MTKMesh?

The parent mesh containing the vertex data of this submesh.

### Properties used to Draw Indexed Primitives

var indexBuffer: MTKMeshBuffer

The index buffer used to render the submesh object.

var indexCount: Int

The number of indices in the index buffer.

var indexType: MTLIndexType

The type of index data in the index buffer.

var primitiveType: MTLPrimitiveType

The primitive type with which to draw the submesh object.

### Identifying Properties

var name: String

The name of the submesh.

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

### Model Handling

class MTKMesh

A container for the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKMeshBuffer

A buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

class MTKMeshBufferAllocator

An interface for allocating a MetalKit buffer that backs the vertex data of a Model I/O mesh, suitable for use in a Metal app.

Conversion Functions

Convert between Metal and Model I/O vertex representations.

Model Errors

Learn about errors thrown by model handling methods.

