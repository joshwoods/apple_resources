

- Core Animation
- CAMetalLayer
-  drawableSize 

Instance Property

# drawableSize

The size, in pixels, of textures for rendering layer content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var drawableSize: CGSize { get set }
```

## Discussion

By default, a layer creates textures sized to match its content—that is, this property’s value is the layer’s bounds size multiplied by its contentsScale factor.

## See Also

### Configuring the Layer’s Drawable Objects

var pixelFormat: MTLPixelFormat

The pixel format of the layer’s textures.

var colorspace: CGColorSpace?

The color space of the rendered content.

var framebufferOnly: Bool

A Boolean value that determines whether the layer’s textures are used only for rendering.

