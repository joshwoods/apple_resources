

- MetalKit
- MTKView
-  framebufferOnly 

Instance Property

# framebufferOnly

A Boolean value that determines whether the drawable’s textures are used only for rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var framebufferOnly: Bool { get set }
```

## Discussion

If the value is true (the default), the underlying CAMetalLayer object allocates its textures with only the renderTarget usage flag. Core Animation can then optimize the textures for display purposes. However, you may not sample, read from, or write to those textures. If the value is false, you can sample or perform read/write operations on the textures, but at a cost to performance.

## See Also

### Configuring the Color Render Target

var colorPixelFormat: MTLPixelFormat

The color pixel format for the current drawable’s texture.

var colorspace: CGColorSpace?

The color space of the rendered content.

var drawableSize: CGSize

The current size of drawable textures.

var preferredDrawableSize: CGSize

The recommended dimensions of the drawable.

var autoResizeDrawable: Bool

A Boolean value that controls whether to resize the drawable as the view changes size.

var clearColor: MTLClearColor

The color to use to clear the color target when creating a render pass descriptor.

