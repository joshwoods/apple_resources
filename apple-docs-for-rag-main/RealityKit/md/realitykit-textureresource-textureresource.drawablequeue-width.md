

- RealityKit
- TextureResource
- TextureResource.DrawableQueue
-  width 

Instance Property

# width

The width of each drawable’s texture in pixels.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var width: Int { get }
```

## See Also

### Working with queues

var allowsNextDrawableTimeout: Bool

A Boolean value that determines whether requests for a new drawable expire if the system can’t satisfy them.

var height: Int

The height of each drawable’s texture in pixels.

var mipmapsMode: TextureResource.MipmapsMode

Options that determine how mipmaps are handled for each drawable’s textures.

var pixelFormat: MTLPixelFormat

The size and bit layout of all pixels in each drawable’s texture.

var usage: MTLTextureUsage

Options that determine how you can use each drawable’s textures.

func nextDrawable() throws -> TextureResource.Drawable

Returns drawable when one is available, blocking the caller in the meantime.

