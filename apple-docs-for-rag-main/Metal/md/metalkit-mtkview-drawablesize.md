

- MetalKit
- MTKView
-  drawableSize 

Instance Property

# drawableSize

The current size of drawable textures.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var drawableSize: CGSize { get set }
```

## Discussion

Changing this value adjusts the size of any color, depth, stencil, and multisampling textures created by the view. If autoResizeDrawable is true, this property is updated automatically whenever the view’s size changes. If autoResizeDrawable is false, set this value to change the size of the texture objects.

The default value is derived from the current view’s size, in native pixels.

## See Also

### Configuring the Color Render Target

var colorPixelFormat: MTLPixelFormat

The color pixel format for the current drawable’s texture.

var colorspace: CGColorSpace?

The color space of the rendered content.

var framebufferOnly: Bool

A Boolean value that determines whether the drawable’s textures are used only for rendering.

var preferredDrawableSize: CGSize

The recommended dimensions of the drawable.

var autoResizeDrawable: Bool

A Boolean value that controls whether to resize the drawable as the view changes size.

var clearColor: MTLClearColor

The color to use to clear the color target when creating a render pass descriptor.

