

- Quartz
- QCRenderer
-  init(offScreenWith:colorSpace:composition:) Deprecated

Initializer

# init(offScreenWith:colorSpace:composition:)

Creates an offscreen renderer of a given size with the provided color space and composition object.

macOS 10.4–10.15Deprecated

``` source
init!(
    offScreenWith size: NSSize,
    colorSpace: CGColorSpace!,
    composition: QCComposition!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`size`  

The size of the offscreen renderer.

`colorSpace`  

A Quartz color space object. This must be an RGB color space. Pass `NULL` to use the default RGB color space. For more information on Quartz color spaces, see Quartz 2D Programming Guide.

`composition`  

A QCComposition object.

## Return Value

The initialized `QCRenderer` object or `nil` if initialization is not successful.

## Discussion

This method creates an internal OpenGL context and pixel buffer. Because offscreen rendering is performed on the GPU, the maximum rendering size is limited to the GPU capacity. On typical hardware, the limit is at least 2048 by 2048, but is often 4096 by 4096. The available VRAM affects performance.

## See Also

### Creating and Initializing a Renderer

init!(composition: QCComposition!, colorSpace: CGColorSpace!)

Creates a renderer object with a composition object and a color space.

Deprecated

init!(openGLContext: NSOpenGLContext!, pixelFormat: NSOpenGLPixelFormat!, file: String!)

Creates a renderer object with an `NSOpenGLContext` object and a composition file.

Deprecated

init!(cglContext: CGLContextObj!, pixelFormat: CGLPixelFormatObj!, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates a renderer object with a `CGLContextObj` object, a pixel format, a color space, and a composition object.

Deprecated

