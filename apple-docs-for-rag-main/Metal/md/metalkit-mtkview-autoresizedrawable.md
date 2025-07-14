

- MetalKit
- MTKView
-  autoResizeDrawable 

Instance Property

# autoResizeDrawable

A Boolean value that controls whether to resize the drawable as the view changes size.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var autoResizeDrawable: Bool { get set }
```

## Discussion

If the value is true, the view automatically resizes its underlying color, depth, stencil, and multisample textures when the view is resized. If the value is false, you must explicitly set drawableSize to change the size of these objects.

The default value is true.

## See Also

### Configuring the Color Render Target

var colorPixelFormat: MTLPixelFormat

The color pixel format for the current drawable’s texture.

var colorspace: CGColorSpace?

The color space of the rendered content.

var framebufferOnly: Bool

A Boolean value that determines whether the drawable’s textures are used only for rendering.

var drawableSize: CGSize

The current size of drawable textures.

var preferredDrawableSize: CGSize

The recommended dimensions of the drawable.

var clearColor: MTLClearColor

The color to use to clear the color target when creating a render pass descriptor.

