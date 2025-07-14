

- Metal
-  MTLTextureSwizzle 

Enumeration

# MTLTextureSwizzle

A set of options to choose from when creating a texture swizzle pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLTextureSwizzle
```

## Topics

### Specifying Swizzle Channels

case alpha

The alpha channel of the source pixel is copied to the destination channel.

case blue

The blue channel of the source pixel is copied to the destination channel.

case green

The green channel of the source pixel is copied to the destination channel.

case red

The red channel of the source pixel is copied to the destination channel.

case one

A value of `1.0` is copied to the destination channel.

case zero

A value of `0.0` is copied to the destination channel.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Texture Attributes

var textureType: MTLTextureType

The dimension and arrangement of texture image data.

var pixelFormat: MTLPixelFormat

The size and bit layout of all pixels in the texture.

var width: Int

The width of the texture image for the base level mipmap, in pixels.

var height: Int

The height of the texture image for the base level mipmap, in pixels.

var depth: Int

The depth of the texture image for the base level mipmap, in pixels.

var mipmapLevelCount: Int

The number of mipmap levels for this texture.

var sampleCount: Int

The number of samples in each fragment.

var arrayLength: Int

The number of array elements for this texture.

var resourceOptions: MTLResourceOptions

The behavior of a new memory allocation.

var cpuCacheMode: MTLCPUCacheMode

The CPU cache mode used for the CPU mapping of the texture.

var storageMode: MTLStorageMode

The location and access permissions of the texture.

var hazardTrackingMode: MTLHazardTrackingMode

The texture’s hazard tracking mode.

var allowGPUOptimizedContents: Bool

A Boolean value indicating whether the GPU is allowed to adjust the texture’s contents to improve GPU performance.

var usage: MTLTextureUsage

Options that determine how you can use the texture.

var swizzle: MTLTextureSwizzleChannels

The pattern you want the GPU to apply to pixels when you read or sample pixels from the texture.

