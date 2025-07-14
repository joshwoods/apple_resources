

- Metal
-  MTLVertexAttributeDescriptorArray 

Class

# MTLVertexAttributeDescriptorArray

An array of vertex attribute descriptor objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexAttributeDescriptorArray
```

## Overview

A MTLVertexAttributeDescriptorArray object is an array of objects that defines how vertex attribute data is formatted and assigned to an index in the attribute argument table. The methods of MTLVertexAttributeDescriptorArray set or retrieve the attribute formatting information from the array.

## Topics

### Accessing a Specified Vertex Attribute

subscript(Int) -> MTLVertexAttributeDescriptor!

Returns the state of the specified vertex attribute.

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

### Render Pass Inputs

class MTLVertexDescriptor

An object that describes how to organize and map data to a vertex function.

class MTLVertexAttributeDescriptor

An object that determines how to store attribute data in memory and map it to the arguments of a vertex function.

class MTLVertexBufferLayoutDescriptor

An object that configures how a render pipeline fetches data to send to the vertex function.

class MTLVertexBufferLayoutDescriptorArray

An array of vertex buffer layout descriptor objects.

let MTLBufferLayoutStrideDynamic: Int

