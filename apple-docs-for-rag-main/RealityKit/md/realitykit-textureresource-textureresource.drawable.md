

- RealityKit
- TextureResource
-  TextureResource.Drawable 

Class

# TextureResource.Drawable

A drawable associated with a drawable queue

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
class Drawable
```

## Topics

### Working with a drawable

var drawableQueue: TextureResource.DrawableQueue

The DrawableQueue that this Drawable is owned by

var texture: any MTLTexture

A Metal texture object that contains the drawable’s contents.

func present()

Presents the updated texture to the renderer as soon as possible.

### Instance Methods

func presentOnSceneUpdate()

Presents the updated texture to the renderer atomically with the current scene update.

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

class DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

struct Descriptor

Describes the texture managed by the drawable queue

