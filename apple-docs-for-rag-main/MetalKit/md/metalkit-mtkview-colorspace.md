

- MetalKit
- MTKView
-  colorspace 

Instance Property

# colorspace

The color space of the rendered content.

macOS 10.12+

``` source
@MainActor
var colorspace: CGColorSpace? { get set }
```

## Discussion

The default value is `nil`, indicating that the rendered content isn’t color-matched. If you set this to a different color space, Core Animation performs any necessary color transformations when compositing the view’s contents.

## See Also

### Configuring the Color Render Target

var colorPixelFormat: MTLPixelFormat

The color pixel format for the current drawable’s texture.

var framebufferOnly: Bool

A Boolean value that determines whether the drawable’s textures are used only for rendering.

var drawableSize: CGSize

The current size of drawable textures.

var preferredDrawableSize: CGSize

The recommended dimensions of the drawable.

var autoResizeDrawable: Bool

A Boolean value that controls whether to resize the drawable as the view changes size.

var clearColor: MTLClearColor

The color to use to clear the color target when creating a render pass descriptor.

