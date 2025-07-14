

- Metal
-  MTLVertexDescriptor 

Class

# MTLVertexDescriptor

An object that describes how to organize and map data to a vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexDescriptor
```

## Overview

A MTLVertexDescriptor object is used to configure how vertex data stored in memory is mapped to attributes in a vertex shader.

A pipeline state is the state of the graphics rendering pipeline, including shaders, blending, multisampling, and visibility testing. For every pipeline state, there can be only one MTLVertexDescriptor object. When you configure a MTLRenderPipelineDescriptor object to create this pipeline state, you use a MTLVertexDescriptor object to establish the vertex layout for the function associated with the pipeline. Create and configure a MTLVertexDescriptor object, then use this object to set the vertexDescriptor property of the MTLRenderPipelineDescriptor object.

## Topics

### Setting Default Values

func reset()

Resets the default state for the vertex descriptor.

### Accessing the Vertex Buffer Layouts and Vertex Attributes

var attributes: MTLVertexAttributeDescriptorArray

An array of state data that describes how vertex attribute data is stored in memory and is mapped to arguments for a vertex shader function.

var layouts: MTLVertexBufferLayoutDescriptorArray

An array of state data that describes how data are fetched by a vertex shader function when rendering primitives.

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

class MTLVertexAttributeDescriptor

An object that determines how to store attribute data in memory and map it to the arguments of a vertex function.

class MTLVertexAttributeDescriptorArray

An array of vertex attribute descriptor objects.

class MTLVertexBufferLayoutDescriptor

An object that configures how a render pipeline fetches data to send to the vertex function.

class MTLVertexBufferLayoutDescriptorArray

An array of vertex buffer layout descriptor objects.

let MTLBufferLayoutStrideDynamic: Int

