

- Quartz
- QCRenderer
-  init(openGLContext:pixelFormat:file:) Deprecated

Initializer

# init(openGLContext:pixelFormat:file:)

Creates a renderer object with an `NSOpenGLContext` object and a composition file.

macOS 10.4–10.15Deprecated

``` source
init!(
    openGLContext context: NSOpenGLContext!,
    pixelFormat format: NSOpenGLPixelFormat!,
    file path: String!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`context`  

An NSOpenGLContext object. The object that you supply must have both a color and a depth buffer.

`format`  

An NSOpenGLPixelFormat object.

`path`  

A string that specifies the location of a composition(`.qtz`) file.

## Return Value

An initialized `QCRenderer` object or `nil` if initialization is not successful.

## See Also

### Creating and Initializing a Renderer

init!(composition: QCComposition!, colorSpace: CGColorSpace!)

Creates a renderer object with a composition object and a color space.

Deprecated

init!(cglContext: CGLContextObj!, pixelFormat: CGLPixelFormatObj!, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates a renderer object with a `CGLContextObj` object, a pixel format, a color space, and a composition object.

Deprecated

init!(offScreenWith: NSSize, colorSpace: CGColorSpace!, composition: QCComposition!)

Creates an offscreen renderer of a given size with the provided color space and composition object.

Deprecated

