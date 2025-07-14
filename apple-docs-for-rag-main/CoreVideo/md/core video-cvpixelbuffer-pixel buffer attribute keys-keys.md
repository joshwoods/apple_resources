

- Core Video
- CVPixelBuffer
-  Pixel Buffer Attribute Keys 

API Collection

# Pixel Buffer Attribute Keys

The attributes associated with a pixel buffer.

## Overview

Use the pixel buffer attribute keys to tell Core Video how to allocate pixel buffers for compatibility with client requirements. A pixel buffer attributes dictionary is a Core Foundation dictionary that contains zero or more key-value pairs. You can pass this dictionary to functions such as CVPixelBufferCreate(_:_:_:_:_:_:) and CVPixelBufferPoolCreate(_:_:_:_:).

To create an attributes dictionary that’s compatible for multiple clients, pass an array of each client’s attributes dictionary to CVPixelBufferCreateResolvedAttributesDictionary(_:_:_:).

## Topics

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

let kCVPixelBufferOpenGLESCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with OpenGL ES contexts.

let kCVPixelBufferMetalCompatibilityKey: CFString

A key to a Boolean value that indicates whether the pixel buffer is compatible with the Metal framework.

let kCVPixelBufferIOSurfaceCoreAnimationCompatibilityKey: CFString

A key to a Boolean value that indicates whether Core Animation can display the pixel buffer.

let kCVPixelBufferIOSurfaceOpenGLFBOCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL can create a valid texture for use as a color buffer attachment.

let kCVPixelBufferIOSurfaceOpenGLESFBOCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL ES can create a valid texture for use as a color buffer attachment.

let kCVPixelBufferIOSurfaceOpenGLTextureCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL can create a valid texture object from the IOSurface-backed pixel buffer.

let kCVPixelBufferIOSurfaceOpenGLESTextureCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL ES can create a valid texture object from the IOSurface-backed pixel buffer.

let kCVPixelBufferOpenGLTextureCacheCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL performs format conversions of the texture-cache data in a shader.

let kCVPixelBufferOpenGLESTextureCacheCompatibilityKey: CFString

A key to a Boolean value that indicates whether OpenGL ES performs format conversions of the texture-cache data in a shader.

