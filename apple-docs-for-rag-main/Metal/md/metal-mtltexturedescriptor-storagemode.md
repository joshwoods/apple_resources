

- Metal
- MTLTextureDescriptor
-  storageMode 

Instance Property

# storageMode

The location and access permissions of the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var storageMode: MTLStorageMode { get set }
```

## Mentioned in 

Optimizing Texture Data

Choosing a Resource Storage Mode for Apple GPUs

## Discussion

In iOS and tvOS, the default value is MTLStorageMode.shared. In macOS, the default value is MTLStorageMode.managed.

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

var hazardTrackingMode: MTLHazardTrackingMode

The texture’s hazard tracking mode.

var allowGPUOptimizedContents: Bool

A Boolean value indicating whether the GPU is allowed to adjust the texture’s contents to improve GPU performance.

var usage: MTLTextureUsage

Options that determine how you can use the texture.

var swizzle: MTLTextureSwizzleChannels

The pattern you want the GPU to apply to pixels when you read or sample pixels from the texture.

struct MTLTextureSwizzleChannels

A pattern that modifies the data read or sampled from a texture by rearranging or duplicating the elements of a vector.

