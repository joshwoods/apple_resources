

- RealityKit
- TextureResource
- TextureResource.Drawable
-  texture 

Instance Property

# texture

A Metal texture object that contains the drawable’s contents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var texture: any MTLTexture { get }
```

## See Also

### Working with a drawable

var drawableQueue: TextureResource.DrawableQueue

The DrawableQueue that this Drawable is owned by

func present()

Presents the updated texture to the renderer as soon as possible.

