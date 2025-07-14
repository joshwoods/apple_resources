

- Metal
-  MTLTextureType 

Enumeration

# MTLTextureType

The dimension of each image, including whether multiple images are arranged into an array or a cube.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLTextureType
```

## Overview

For a `MTLTextureTypeCube` texture, the property values describe one slice, which is any one of its six sides. For example, mipmapLevelCount is the number of mipmap levels for one slice, not the total sum of mipmap levels in six slices. By definition, the width and height of a cube texture are the same value.

Each slice of a cube texture maps to a side with a specific orientation.

| Slice index | Slice orientation |
|-------------|-------------------|
| 0           | +X                |
| 1           | -X                |
| 2           | +Y                |
| 3           | -Y                |
| 4           | +Z                |
| 5           | -Z                |

## Topics

### Specifying the Texture Type

case type1D

A one-dimensional texture image.

case type1DArray

An array of one-dimensional texture images.

case type2D

A two-dimensional texture image.

case type2DArray

An array of two-dimensional texture images.

case type2DMultisample

A two-dimensional texture image that uses more than one sample for each pixel.

case typeCube

A cube texture with six two-dimensional images.

case typeCubeArray

An array of cube textures, each with six two-dimensional images.

case type3D

A three-dimensional texture image.

case type2DMultisampleArray

An array of two-dimensional texture images that use more than one sample for each pixel.

case typeTextureBuffer

A texture buffer.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Querying Texture Attributes

var textureType: MTLTextureType

The dimension and arrangement of the texture image data.

**Required**

var pixelFormat: MTLPixelFormat

The format of pixels in the texture.

**Required**

var width: Int

The width of the texture image for the base level mipmap, in pixels.

**Required**

var height: Int

The height of the texture image for the base level mipmap, in pixels.

**Required**

var depth: Int

The depth of the texture image for the base level mipmap, in pixels.

**Required**

var mipmapLevelCount: Int

The number of mipmap levels in the texture.

**Required**

var arrayLength: Int

The number of slices in the texture array.

**Required**

var sampleCount: Int

The number of samples in each pixel.

**Required**

var isFramebufferOnly: Bool

A Boolean value that indicates whether the texture can only be used as a render target.

**Required**

var usage: MTLTextureUsage

Options that determine how you can use the texture.

**Required**

var allowGPUOptimizedContents: Bool

A Boolean value indicating whether the GPU is allowed to adjust the contents of the texture to improve GPU performance.

**Required**

var isShareable: Bool

A Boolean indicating whether this texture can be shared with other processes.

**Required**

var swizzle: MTLTextureSwizzleChannels

The pattern that the GPU applies to pixels when you read or sample pixels from the texture.

**Required**

struct MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

