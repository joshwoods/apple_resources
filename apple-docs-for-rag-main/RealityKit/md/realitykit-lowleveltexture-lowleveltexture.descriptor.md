

- RealityKit
- LowLevelTexture
-  LowLevelTexture.Descriptor 

Structure

# LowLevelTexture.Descriptor

An object that you use to configure new `LowLevelTexture` objects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Descriptor
```

## Topics

### Initializers

init(textureType: MTLTextureType, pixelFormat: MTLPixelFormat, width: Int, height: Int, depth: Int, mipmapLevelCount: Int, arrayLength: Int, textureUsage: MTLTextureUsage, swizzle: MTLTextureSwizzleChannels)

Creates a descriptor for a low-level texture.

### Instance Properties

var arrayLength: Int

The number of array elements for this texture.

var depth: Int

The depth of the texture image for the base level mipmap, in pixels.

var height: Int

The height of the texture image for the base level mipmap, in pixels.

var mipmapLevelCount: Int

The number of mipmap levels for the texture.

var pixelFormat: MTLPixelFormat

The size and bit layout of all pixels in the texture.

var swizzle: MTLTextureSwizzleChannels

The pattern you want the GPU to apply to pixels when you read or sample pixels from the texture.

var textureType: MTLTextureType

The dimension and arrangement of texture image data.

var textureUsage: MTLTextureUsage

An enumeration for the various options that determine how you can use a texture.

var width: Int

The width of the texture image for the base level mipmap, in pixels.

## See Also

### Texture drawing

Rendering a windowed game in stereo

Bring an iOS or iPadOS game to visionOS and enhance it.

Creating a dynamic height and normal map with low-level texture

Create a low-level texture and update its pixel data on the GPU to form a dynamic height and normal map.

class LowLevelTexture

A container for texture data allowing you to create and update textures using your own format.

class Drawable

A drawable associated with a drawable queue

class DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

struct Descriptor

Describes the texture managed by the drawable queue

