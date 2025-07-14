

- MetalKit
- MTKView
-  colorPixelFormat 

Instance Property

# colorPixelFormat

The color pixel format for the current drawable’s texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var colorPixelFormat: MTLPixelFormat { get set }
```

## Discussion

The pixel format must be one that the underlying CAMetalLayer can use. See pixelFormat.

The default value is MTLPixelFormat.bgra8Unorm.

## See Also

### Configuring the Color Render Target

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

var clearColor: MTLClearColor

The color to use to clear the color target when creating a render pass descriptor.

