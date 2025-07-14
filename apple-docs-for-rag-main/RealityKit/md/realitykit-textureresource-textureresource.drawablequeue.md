

- RealityKit
- TextureResource
-  TextureResource.DrawableQueue 

Class

# TextureResource.DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
class DrawableQueue
```

## Overview

Each drawable queue can work with at most one consumer, such as a RealityRenderer instance or a render server.

## Topics

### Creating a queue

init(TextureResource.DrawableQueue.Descriptor) throws

Create a new drawable queue.

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

var width: Int

The width of each drawable’s texture in pixels.

func nextDrawable() throws -> TextureResource.Drawable

Returns drawable when one is available, blocking the caller in the meantime.

### Structures

struct Descriptor

Describes the texture managed by the drawable queue

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

struct Descriptor

Describes the texture managed by the drawable queue

