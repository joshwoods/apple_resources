

- Metal
-  MTLArgumentDescriptor 

Class

# MTLArgumentDescriptor

A representation of an argument within an argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLArgumentDescriptor
```

## Overview

This descriptor can represent arguments within flat structures only. It can represent arrays of allowed argument buffer data types, but it cannot represent arguments within nested structures. Argument buffers with simple, flat structures can be represented by an array of MTLArgumentDescriptor objects. You can then use this array to create a MTLArgumentEncoder object by calling the makeArgumentEncoder(arguments:) method.Argument buffers with complex, nested structures must define their structure in Metal shading language code, which can then be directly assigned to a specific buffer index of a function. You can then use this buffer index to call the makeArgumentEncoder(bufferIndex:) method and create a MTLArgumentEncoder object.

## Topics

### Setting the Descriptor’s Properties

var dataType: MTLDataType

The data type of the argument.

var index: Int

The index ID of the argument.

var access: MTLBindingAccess

The access permissions of the argument.

var arrayLength: Int

The length of an array argument.

var constantBlockAlignment: Int

The alignment of the constant block.

var textureType: MTLTextureType

The texture type of a texture argument.

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

### Argument Buffers

Improving CPU Performance by Using Argument Buffers

Optimize your app’s performance by grouping your resources into argument buffers.

Managing groups of resources with argument buffers

Create argument buffers to organize related resources.

Tracking the Resource Residency of Argument Buffers

Optimize resource performance within an argument buffer.

Indexing Argument Buffers

Assign resource indices within an argument buffer.

Rendering Terrain Dynamically with Argument Buffers

Use argument buffers to render terrain in real time with a GPU-driven pipeline.

Encoding Argument Buffers on the GPU

Use a compute pass to encode an argument buffer and access its arguments in a subsequent render pass.

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

protocol MTLArgumentEncoder

An object used to encode data into an argument buffer.

let MTLAttributeStrideStatic: Int

