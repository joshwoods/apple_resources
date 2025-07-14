

- Metal
- MTLTexture
-  allowGPUOptimizedContents 

Instance Property

# allowGPUOptimizedContents

A Boolean value indicating whether the GPU is allowed to adjust the contents of the texture to improve GPU performance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var allowGPUOptimizedContents: Bool { get }
```

**Required**

## Discussion

The value is set when the texture is created and never changes.

If the value is `true`, Metal is allowed to adjust the texture’s contents to improve GPU performance. For a shared or managed texture, this optimization can cause slower performance when accessing the texture from the CPU. If the value is `false`, CPU reads and writes may be improved at the cost of some GPU performance.

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

var isShareable: Bool

A Boolean indicating whether this texture can be shared with other processes.

**Required**

var swizzle: MTLTextureSwizzleChannels

The pattern that the GPU applies to pixels when you read or sample pixels from the texture.

**Required**

enum MTLTextureType

The dimension of each image, including whether multiple images are arranged into an array or a cube.

struct MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

