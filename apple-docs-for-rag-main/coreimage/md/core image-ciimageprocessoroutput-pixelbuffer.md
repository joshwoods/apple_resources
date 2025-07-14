

- Core Image
- CIImageProcessorOutput
-  pixelBuffer 

Instance Property

# pixelBuffer

A CoreVideo pixel buffer to which you can write output pixel data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var pixelBuffer: CVPixelBuffer? { get }
```

**Required**

## Discussion

Use this property to process the image using routines that can make use of memory shared with Core Video. For example, if your image processing technology uses OpenGL or OpenGL ES, you can create a GL texture from a Core Video pixel buffer with the CVOpenGLBufferPool or CVOpenGLESTextureCache API.

## See Also

### Providing Output Image Data

var baseAddress: UnsafeMutableRawPointer

A pointer to CPU memory at which to write output pixel data.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture to which you can write output pixel data.

**Required**

var surface: IOSurfaceRef

An IOSurface object to which you can write output pixel data.

**Required**

