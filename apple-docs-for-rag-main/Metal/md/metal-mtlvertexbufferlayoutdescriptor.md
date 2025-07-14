

- Metal
-  MTLVertexBufferLayoutDescriptor 

Class

# MTLVertexBufferLayoutDescriptor

An object that configures how a render pipeline fetches data to send to the vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexBufferLayoutDescriptor
```

## Topics

### Organizing the Vertex Buffer Layout

var stepFunction: MTLVertexStepFunction

The circumstances under which the vertex and its attributes are presented to the vertex function.

var stepRate: Int

The interval at which the vertex and its attributes are presented to the vertex function.

var stride: Int

The number of bytes between the first byte of two consecutive vertices in a buffer.

### Constants

enum MTLVertexStepFunction

The frequency with which the vertex function or post-tessellation vertex function fetches attribute data.

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

class MTLVertexAttributeDescriptor

An object that determines how to store attribute data in memory and map it to the arguments of a vertex function.

class MTLVertexAttributeDescriptorArray

An array of vertex attribute descriptor objects.

class MTLVertexBufferLayoutDescriptorArray

An array of vertex buffer layout descriptor objects.

let MTLBufferLayoutStrideDynamic: Int

