

- MetalKit
- MTKView
-  clearColor 

Instance Property

# clearColor

The color to use to clear the color target when creating a render pass descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var clearColor: MTLClearColor { get set }
```

## Discussion

When the view creates a render pass, it sets the load action for the color render target to MTLLoadAction.clear and uses this color as the clear color. The default value is `(0.0, 0.0, 0.0, 1.0)`.

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

var autoResizeDrawable: Bool

A Boolean value that controls whether to resize the drawable as the view changes size.

