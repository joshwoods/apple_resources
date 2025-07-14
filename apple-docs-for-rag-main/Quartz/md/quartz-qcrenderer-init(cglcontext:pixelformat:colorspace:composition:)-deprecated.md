

- Quartz
- QCRenderer
-  init(cglContext:pixelFormat:colorSpace:composition:) Deprecated

Initializer

# init(cglContext:pixelFormat:colorSpace:composition:)

Creates a renderer object with a `CGLContextObj` object, a pixel format, a color space, and a composition object.

macOS 10.5–10.14Deprecated

``` source
init!(
    cglContext context: CGLContextObj!,
    pixelFormat format: CGLPixelFormatObj!,
    colorSpace: CGColorSpace!,
    composition: QCComposition!
)
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`context`  

A `CGLContextObj` object. The object that you supply must have both a color and a depth buffer.

`format`  

A `CGLPixelFormatObj` object.

`colorSpace`  

A Quartz color space object. This must be an RGB color space. Pass `NULL` to use the default RGB color space. For more information on Quartz color spaces, see Quartz 2D Programming Guide.

`composition`  

A QCComposition object.

## Return Value

The initialized `QCRenderer` object or `nil` if initialization is not successful.

## See Also

### Creating and Initializing a Renderer

init!(composition: QCComposition!, colorSpace: CGColorSpace!)

Creates a renderer object with a composition object and a color space.

Deprecated

init!(openGLContext: NSOpenGLContext!, pixelFormat: NSOpenGLPixelFormat!, file: String!)

Creates a renderer object with an `NSOpenGLContext` object and a composition file.

Deprecated

init!(offScreenWith: NSSize, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates an offscreen renderer of a given size with the provided color space and composition object.

Deprecated

