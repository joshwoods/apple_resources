

- Metal
-  MTLArgument Deprecated

Class

# MTLArgument

Information about an argument of a graphics or compute function.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MTLArgument
```

## Overview

A MTLArgument object describes a single argument to a Metal function. Your app uses the MTLArgument properties to read details about a function argument as it was defined in the Metal Shading Language. You can determine the argument’s data type, access restrictions, and its associated resource type. For buffer, texture, and threadgroup memory arguments, additional properties can be read to determine more details about the argument.

Your app does not create a MTLArgument object directly. Creating a MTLRenderPipelineState or MTLComputePipelineState object can generate a reflection object (MTLRenderPipelineReflection or MTLComputePipelineReflection) that contains MTLArgument objects.

## Topics

### Describing the Argument

var name: String

The name of the argument.

var isActive: Bool

A Boolean that indicates whether the compiled function uses the argument.

var index: Int

The index in the argument table that corresponds to the function argument.

var type: MTLArgumentType

The argument’s resource type.

var access: MTLBindingAccess

The argument’s read and/or write access.

### Describing a Buffer Argument

var bufferAlignment: Int

The required byte alignment in memory for the buffer data.

var bufferDataSize: Int

The size, in bytes, of the buffer data.

var bufferDataType: MTLDataType

The data type of the buffer data.

var bufferStructType: MTLStructType?

A description of the structure data of a buffer argument.

var bufferPointerType: MTLPointerType?

A description of the pointer to a buffer argument.

### Describing a Texture Argument

var textureDataType: MTLDataType

The data type of a texture argument.

var textureType: MTLTextureType

The texture type of a texture argument.

var isDepthTexture: Bool

A Boolean value that indicates whether the texture is a depth texture.

### Describing an Array Argument

var arrayLength: Int

The number of elements, if the argument is an array.

### Describing a Threadgroup Memory Argument

var threadgroupMemoryAlignment: Int

The required byte alignment in memory for the threadgroup data.

var threadgroupMemoryDataSize: Int

The size, in bytes, of the threadgroup data.

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

### Function Arguments

class MTLAttribute

An object that describes an attribute defined in the stage-in argument for a shader.

class MTLVertexAttribute

An object that represents an attribute of a vertex function.

typealias MTLAutoreleasedArgument

A convenience type alias for an autoreleased argument instance.

Deprecated

enum MTLArgumentType

The resource type for an argument of a function.

Deprecated

typealias MTLArgumentAccess

Function access restrictions to argument data in the shading language code.

Deprecated

