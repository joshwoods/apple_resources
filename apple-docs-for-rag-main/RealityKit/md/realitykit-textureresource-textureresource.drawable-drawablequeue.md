

- RealityKit
- TextureResource
- TextureResource.Drawable
-  drawableQueue 

Instance Property

# drawableQueue

The DrawableQueue that this Drawable is owned by

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var drawableQueue: TextureResource.DrawableQueue { get }
```

## See Also

### Working with a drawable

var texture: any MTLTexture

A Metal texture object that contains the drawable’s contents.

func present()

Presents the updated texture to the renderer as soon as possible.

