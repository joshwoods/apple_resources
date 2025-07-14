

- Core Animation
- CAMetalLayer
-  colorspace 

Instance Property

# colorspace

The color space of the rendered content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var colorspace: CGColorSpace? { get set }
```

## Discussion

Set this value to specify a color space for the contents of the layer. When a color space is present, Core Animation performs any necessary color space transformations when compositing this content.

The default value is `nil`, indicating that the rendered content isn’t color-matched.

## See Also

### Configuring the Layer’s Drawable Objects

var pixelFormat: MTLPixelFormat

The pixel format of the layer’s textures.

var framebufferOnly: Bool

A Boolean value that determines whether the layer’s textures are used only for rendering.

var drawableSize: CGSize

The size, in pixels, of textures for rendering layer content.

