

- Core Animation
- CAMetalLayer
-  pixelFormat 

Instance Property

# pixelFormat

The pixel format of the layer’s textures.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var pixelFormat: MTLPixelFormat { get set }
```

## Discussion

The default value is MTLPixelFormat.bgra8Unorm.

You must use one of the following formats:

- MTLPixelFormat.bgra8Unorm

- MTLPixelFormat.bgra8Unorm_srgb

- MTLPixelFormat.rgba16Float

- MTLPixelFormat.rgb10a2Unorm

- MTLPixelFormat.bgr10a2Unorm

- MTLPixelFormat.bgra10_xr

- MTLPixelFormat.bgra10_xr_srgb

- MTLPixelFormat.bgr10_xr

- MTLPixelFormat.bgr10_xr_srgb

## See Also

### Configuring the Layer’s Drawable Objects

var colorspace: CGColorSpace?

The color space of the rendered content.

var framebufferOnly: Bool

A Boolean value that determines whether the layer’s textures are used only for rendering.

var drawableSize: CGSize

The size, in pixels, of textures for rendering layer content.

