

- Metal
- MTLTextureDescriptor
-  allowGPUOptimizedContents 

Instance Property

# allowGPUOptimizedContents

A Boolean value indicating whether the GPU is allowed to adjust the texture’s contents to improve GPU performance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var allowGPUOptimizedContents: Bool { get set }
```

## Mentioned in 

Optimizing Texture Data

## Discussion

The default value is `true`, which means that the Metal device is allowed to adjust the private layout of the texture in memory to improve GPU performance. For a shared or managed texture, this optimization can cause slower performance when accessing the texture from the CPU. Setting this property to `false` improves CPU performance at the cost of some GPU performance.

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

var usage: MTLTextureUsage

Options that determine how you can use the texture.

var swizzle: MTLTextureSwizzleChannels

The pattern you want the GPU to apply to pixels when you read or sample pixels from the texture.

struct MTLTextureSwizzleChannels

A pattern that modifies the data read or sampled from a texture by rearranging or duplicating the elements of a vector.

