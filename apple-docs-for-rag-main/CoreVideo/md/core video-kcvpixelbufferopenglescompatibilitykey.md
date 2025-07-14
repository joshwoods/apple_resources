

- Core Video
-  kCVPixelBufferOpenGLESCompatibilityKey 

Global Variable

# kCVPixelBufferOpenGLESCompatibilityKey

A key to a Boolean value that indicates whether the pixel buffer is compatible with OpenGL ES contexts.

iOS 6.0+iPadOS 6.0+tvOS 9.0+

``` source
let kCVPixelBufferOpenGLESCompatibilityKey: CFString
```

## Discussion

The value for this key is of type CFBoolean. To use pixel buffers in OpenGL ES rendering, see CVOpenGLESTextureCache.

## See Also

### Constants

let kCVPixelBufferMemoryAllocatorKey: CFString

A key to the allocator that the system uses to create the pixel buffer.

let kCVPixelBufferPixelFormatTypeKey: CFString

A key to one or more pixel buffer format types.

let kCVPixelBufferWidthKey: CFString

A key to the width of the pixel buffer.

let kCVPixelBufferHeightKey: CFString

A key to the height of the pixel buffer.

let kCVPixelBufferExtendedPixelsLeftKey: CFString

A key to the number of pixels padding the left of the image.

let kCVPixelBufferExtendedPixelsTopKey: CFString

A key to the number of pixels padding the top of the image.

let kCVPixelBufferExtendedPixelsRightKey: CFString

A key to the number of pixels padding the right of the image.

let kCVPixelBufferExtendedPixelsBottomKey: CFString

A key to the number of pixels padding the bottom of the image.

let kCVPixelBufferBytesPerRowAlignmentKey: CFString

A key to a number that specifies the alignment of number of bytes per row in the pixel buffer.

let kCVPixelBufferCGBitmapContextCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with Core Graphics bitmap contexts.

let kCVPixelBufferCGImageCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with Core Graphics bitmap image types.

let kCVPixelBufferOpenGLCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with OpenGL contexts.

let kCVPixelBufferPlaneAlignmentKey: CFString

A key to a number that specifies the alignment of the planes in the pixel buffer.

let kCVPixelBufferIOSurfacePropertiesKey: CFString

A key to the dictionary containing optional properties for the IOSurface framework.

let kCVPixelBufferMetalCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with the Metal framework.

