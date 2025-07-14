

- RealityKit
- TextureResource
- TextureResource.Drawable
-  present() 

Instance Method

# present()

Presents the updated texture to the renderer as soon as possible.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func present()
```

## Discussion

Needs to be called after all commands in the command buffer have been executed (e.g. after `MTLCommandBuffer.waitUntilCompleted()`). When you call this method, the drawable will make the new texture content available to the renderer immediately.

Alternatively, instead of waiting for completion you can call `MTLCommandBuffer.present(_:)` to signal in the command buffer that the texture is ready to use.

## See Also

### Working with a drawable

var drawableQueue: TextureResource.DrawableQueue

The DrawableQueue that this Drawable is owned by

var texture: any MTLTexture

A Metal texture object that contains the drawable’s contents.

