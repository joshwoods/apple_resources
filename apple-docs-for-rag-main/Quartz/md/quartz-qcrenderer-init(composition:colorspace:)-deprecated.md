

- Quartz
- QCRenderer
-  init(composition:colorSpace:) Deprecated

Initializer

# init(composition:colorSpace:)

Creates a renderer object with a composition object and a color space.

macOS 10.4–10.15Deprecated

``` source
init!(
    composition: QCComposition!,
    colorSpace: CGColorSpace!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`composition`  

A QCComposition object. The composition must not contain any consumer patches. That is, the composition can receive data, process it, and produce output values, but it cannot perform any rendering.

`colorSpace`  

A Quartz color space object. This must be an RGB color space. Pass `NULL` to use the default RGB color space. The color space is used only for the images produced by the output image ports of the composition. For more information on Quartz color spaces, see Quartz 2D Programming Guide.

## Return Value

The initialized `QCRenderer` object or `nil` if initialization is not successful.

## Discussion

Note that snapshotImage() and createSnapshotImage(ofType:) always returns `nil` on such `QCRenderer` instances.

## See Also

### Creating and Initializing a Renderer

init!(openGLContext: NSOpenGLContext!, pixelFormat: NSOpenGLPixelFormat!, file: String!)

Creates a renderer object with an `NSOpenGLContext` object and a composition file.

Deprecated

init!(cglContext: CGLContextObj!, pixelFormat: CGLPixelFormatObj!, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates a renderer object with a `CGLContextObj` object, a pixel format, a color space, and a composition object.

Deprecated

init!(offScreenWith: NSSize, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates an offscreen renderer of a given size with the provided color space and composition object.

Deprecated

