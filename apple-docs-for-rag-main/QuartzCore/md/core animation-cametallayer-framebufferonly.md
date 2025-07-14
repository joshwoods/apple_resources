

- Core Animation
- CAMetalLayer
-  framebufferOnly 

Instance Property

# framebufferOnly

A Boolean value that determines whether the layer’s textures are used only for rendering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var framebufferOnly: Bool { get set }
```

## Discussion

If the value is true (the default), the CAMetalLayer class allocates its MTLTexture objects with only the renderTarget usage flag. Core Animation can then optimize the texture for display purposes. However, you may not sample, read from, or write to those textures. To support sampling and pixel read/write operations (at a cost to performance), set this value to false.

## See Also

### Configuring the Layer’s Drawable Objects

var pixelFormat: MTLPixelFormat

The pixel format of the layer’s textures.

var colorspace: CGColorSpace?

The color space of the rendered content.

var drawableSize: CGSize

The size, in pixels, of textures for rendering layer content.

