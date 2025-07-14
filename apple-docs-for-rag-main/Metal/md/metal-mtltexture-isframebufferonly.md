

- Metal
- MTLTexture
-  isFramebufferOnly 

Instance Property

# isFramebufferOnly

A Boolean value that indicates whether the texture can only be used as a render target.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var isFramebufferOnly: Bool { get }
```

**Required**

## Discussion

The default is false, which indicates the use of the texture is not restricted.

If true, neither replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) nor getBytes(_:bytesPerRow:bytesPerImage:from:mipmapLevel:slice:) can be used with this texture. Also, this texture can only be used as an attachment for MTLRenderPassDescriptor and cannot be a texture argument for MTLRenderCommandEncoder, MTLBlitCommandEncoder, or MTLComputeCommandEncoder.

Textures obtained from a CAMetalDrawable object may only be usable as attachments, depending on the value of framebufferOnly passed to their parent CAMetalLayer object. Textures created directly by the app do not have such restrictions.

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

