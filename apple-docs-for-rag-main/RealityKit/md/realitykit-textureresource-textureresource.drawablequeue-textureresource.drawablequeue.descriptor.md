

- RealityKit
- TextureResource
- TextureResource.DrawableQueue
-  TextureResource.DrawableQueue.Descriptor 

Structure

# TextureResource.DrawableQueue.Descriptor

Describes the texture managed by the drawable queue

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Descriptor
```

## Topics

### Initializers

init(pixelFormat: MTLPixelFormat, width: Int, height: Int, usage: MTLTextureUsage, mipmapsMode: TextureResource.MipmapsMode)

init(pixelFormat: MTLPixelFormat, width: Int, height: Int, usage: MTLTextureUsage, mipmapsMode: TextureResource.MipmapsMode, timeout: Duration)

### Instance Properties

var height: Int

The height of each drawable’s texture in pixels.

var mipmapsMode: TextureResource.MipmapsMode

A Boolean value that determines whether the resource should generate mipmaps for each drawable’s texture after it was updated.

var pixelFormat: MTLPixelFormat

The size and bit layout of all pixels in each drawable’s texture.

var timeout: Duration

Specifies a timeout value in seconds when querying nextDrawable(). nextDrawable() will be blocked for up to the specified timeout period for a drawable to become available else throws `NextDrawableError.timeoutReached`. By default this is set to 1 second. Note that if `allowsNextDrawableTimeout` is false, then the timeout parameter will be ignored.

var usage: MTLTextureUsage

Options that determine how you can use each drawable’s textures.

var width: Int

The width of each drawable’s texture in pixels.

## See Also

### Texture drawing

Rendering a windowed game in stereo

Bring an iOS or iPadOS game to visionOS and enhance it.

Creating a dynamic height and normal map with low-level texture

Create a low-level texture and update its pixel data on the GPU to form a dynamic height and normal map.

class LowLevelTexture

A container for texture data allowing you to create and update textures using your own format.

struct Descriptor

An object that you use to configure new `LowLevelTexture` objects.

class Drawable

A drawable associated with a drawable queue

class DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

