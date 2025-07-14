

- Metal
- MTLTexture
-  arrayLength 

Instance Property

# arrayLength

The number of slices in the texture array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var arrayLength: Int { get }
```

**Required**

## Discussion

The value of this property ranges from 1 to 2048, inclusive. If the texture type is not an array, this value is 1.

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

enum MTLTextureType

The dimension of each image, including whether multiple images are arranged into an array or a cube.

struct MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

