

- Metal
-  MTLVertexBufferLayoutDescriptorArray 

Class

# MTLVertexBufferLayoutDescriptorArray

An array of vertex buffer layout descriptor objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexBufferLayoutDescriptorArray
```

## Overview

A MTLVertexBufferLayoutDescriptorArray holds an array of vertex buffer layout states. The methods of MTLVertexBufferLayoutDescriptorArray set the vertex buffer layout state in the array or retrieve the state from the array.

## Topics

### Accessing a Specified Vertex Buffer Layout

subscript(Int) -> MTLVertexBufferLayoutDescriptor!

Returns the state of the specified vertex buffer layout.

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

class MTLVertexAttributeDescriptorArray

An array of vertex attribute descriptor objects.

class MTLVertexBufferLayoutDescriptor

An object that configures how a render pipeline fetches data to send to the vertex function.

let MTLBufferLayoutStrideDynamic: Int

