

- Metal
-  MTLVertexAttributeDescriptor 

Class

# MTLVertexAttributeDescriptor

An object that determines how to store attribute data in memory and map it to the arguments of a vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexAttributeDescriptor
```

## Overview

A vertex attribute descriptor provides organization information so a vertex shader function can locate and load data into its arguments. The descriptor maps memory locations to attribute locations. It supports access to multiple attributes (such as vertex coordinates, surface normals, and texture coordinates) that are interleaved within the same buffer.

## Topics

### Organizing the Vertex Attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var bufferIndex: Int

The index in the argument table for the associated vertex buffer.

### Constants

enum MTLVertexFormat

Values that specify the organization of function vertex data.

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

### Render Pass Inputs

class MTLVertexDescriptor

An object that describes how to organize and map data to a vertex function.

class MTLVertexAttributeDescriptorArray

An array of vertex attribute descriptor objects.

class MTLVertexBufferLayoutDescriptor

An object that configures how a render pipeline fetches data to send to the vertex function.

class MTLVertexBufferLayoutDescriptorArray

An array of vertex buffer layout descriptor objects.

let MTLBufferLayoutStrideDynamic: Int

