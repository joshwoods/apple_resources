

- Metal
-  MTLSamplerDescriptor 

Class

# MTLSamplerDescriptor

An object that you use to configure a texture sampler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLSamplerDescriptor
```

## Mentioned in 

Restricting Access to Specific Mipmaps

Adding Mipmap Filtering to Samplers

Improving CPU Performance by Using Argument Buffers

## Overview

To make a sampler, create and configure an MTLSamplerDescriptor instance and then call an MTLDevice instance’s makeSamplerState(descriptor:) method. After you create the sampler, you can release the descriptor or reconfigure its properties to create other samplers.

## Topics

### Declaring the Coordinate Space

var normalizedCoordinates: Bool

A Boolean value that indicates whether texture coordinates are normalized to the range `[0.0, 1.0]`.

### Declaring Addressing Modes

var rAddressMode: MTLSamplerAddressMode

The address mode for the texture depth (r) coordinate.

var sAddressMode: MTLSamplerAddressMode

The address mode for the texture width (s) coordinate.

var tAddressMode: MTLSamplerAddressMode

The address mode for the texture height (t) coordinate.

var borderColor: MTLSamplerBorderColor

The border color for clamped texture values.

enum MTLSamplerAddressMode

Modes that determine the texture coordinate at each pixel when a fetch falls outside the bounds of a texture.

enum MTLSamplerBorderColor

Values that determine the border color for clamped texture values when the sampler address mode is MTLSamplerAddressMode.clampToBorderColor.

### Declaring Filter Modes

var minFilter: MTLSamplerMinMagFilter

The filtering option for combining pixels within one mipmap level when the sample footprint is larger than a pixel (minification).

var magFilter: MTLSamplerMinMagFilter

The filtering operation for combining pixels within one mipmap level when the sample footprint is smaller than a pixel (magnification).

var mipFilter: MTLSamplerMipFilter

The filtering option for combining pixels between two mipmap levels.

var lodMinClamp: Float

The minimum level of detail (LOD) to use when sampling from a texture.

var lodMaxClamp: Float

The maximum level of detail (LOD) to use when sampling from a texture.

var lodAverage: Bool

A Boolean value that specifies whether the GPU can use an average level of detail (LOD) when sampling from a texture.

var maxAnisotropy: Int

The number of samples that can be taken to improve the quality of sample footprints that are anisotropic.

enum MTLSamplerMinMagFilter

Filtering options for determining which pixel value is returned within a mipmap level.

enum MTLSamplerMipFilter

Filtering options for determining what pixel value is returned with multiple mipmap levels.

### Declaring the Depth Comparison Mode

var compareFunction: MTLCompareFunction

The sampler comparison function used when performing a sample compare operation on a depth texture.

enum MTLCompareFunction

Options used to specify how a sample compare operation should be performed on a depth texture.

### Declaring Whether the Sampler Can Be Used in Argument Buffers

var supportArgumentBuffers: Bool

A Boolean value that indicates whether you can reference a sampler, that you make with this descriptor, by its resource ID from an argument buffer.

### Identifying the Sampler

var label: String?

A string that identifies the sampler.

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

### Texture Samplers

Creating and Sampling Textures

Load image data into a texture and apply it to a quadrangle.

protocol MTLSamplerState

An object that defines how a texture should be sampled.

struct MTLSamplePosition

A subpixel sample position for use in multisample antialiasing (MSAA).

