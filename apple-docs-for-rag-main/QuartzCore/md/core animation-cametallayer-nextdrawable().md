

- Core Animation
- CAMetalLayer
-  nextDrawable() 

Instance Method

# nextDrawable()

Waits until a Metal drawable is available, and then returns it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextDrawable() -> (any CAMetalDrawable)?
```

## Return Value

A Metal drawable. Use the drawable’s texture property to configure a MTLRenderPipelineColorAttachmentDescriptor object for rendering to the layer.

## Discussion

A CAMetalLayer object maintains an internal pool of textures for displaying layer content, each wrapped in a CAMetalDrawable object. Use this method to retrieve the next available drawable from the pool. If all drawables are in use, the layer waits up to one second for one to become available, after which it returns `nil`. The allowsNextDrawableTimeout property affects this behavior.

This method returns `nil` if the layer’s pixelFormat or other properties are invalid.

## See Also

### Obtaining a Metal Drawable

var maximumDrawableCount: Int

The number of Metal drawables in the resource pool managed by Core Animation.

var allowsNextDrawableTimeout: Bool

A Boolean value that determines whether requests for a new buffer expire if the system can’t satisfy them.

