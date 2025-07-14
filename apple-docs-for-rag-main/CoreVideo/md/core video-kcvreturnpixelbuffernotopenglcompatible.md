

- Core Video
-  kCVReturnPixelBufferNotOpenGLCompatible 

Global Variable

# kCVReturnPixelBufferNotOpenGLCompatible

The pixel buffer is not compatible with OpenGL due to an unsupported buffer size, pixel format, or attribute.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var kCVReturnPixelBufferNotOpenGLCompatible: CVReturn { get }
```

## See Also

### Pixel Buffer

var kCVReturnInvalidPixelBufferAttributes: CVReturn

A buffer cannot be created with the specified attributes.

var kCVReturnInvalidPixelFormat: CVReturn

The buffer does not support the specified pixel format.

var kCVReturnInvalidSize: CVReturn

The buffer cannot support the requested buffer size (usually too big).

var kCVReturnPixelBufferNotMetalCompatible: CVReturn

The pixel buffer is not compatible with Metal due to an unsupported buffer size, pixel format, or attribute.

