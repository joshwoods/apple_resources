

- Core Image
- CIImageProcessorInput
-  pixelBuffer 

Instance Property

# pixelBuffer

A CoreVideo pixel buffer containing the image data to be processed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var pixelBuffer: CVPixelBuffer? { get }
```

**Required**

## Discussion

Use this property if you plan to process the image using routines that can make use of memory shared with Core Video. For example, if your image processing technology uses OpenGL or OpenGL ES, you can create a GL texture from a Core Video pixel buffer with the CVOpenGLBufferPool or CVOpenGLESTextureCache API.

Do not modify the contents of this buffer.

## See Also

### Accessing Input Image Data

var baseAddress: UnsafeRawPointer

A pointer to the image data in CPU memory to be processed.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture containing the image data to be processed.

**Required**

var surface: IOSurfaceRef

An IOSurface object containing the image data to be processed.

**Required**

