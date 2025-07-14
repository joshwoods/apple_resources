

- Core Video
-  CVPixelBufferCreate(\_:\_:\_:\_:\_:\_:) 

Function

# CVPixelBufferCreate(\_:\_:\_:\_:\_:\_:)

Creates a single pixel buffer for a given size and pixel format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferCreate(
    _ allocator: CFAllocator?,
    _ width: Int,
    _ height: Int,
    _ pixelFormatType: OSType,
    _ pixelBufferAttributes: CFDictionary?,
    _ pixelBufferOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The allocator to use for creating the buffer pool. Pass kCFAllocatorDefault for the `allocator` parameter to use the default allocator. See Predefined Allocators for additional values you can use.

`width`  

The width of the pixel buffer, in pixels.

`height`  

The height of the pixel buffer, in pixels.

`pixelFormatType`  

The pixel format identified by its four-character code.

`pixelBufferAttributes`  

An optional dictionary that contains the attributes for the pixel buffer. See Pixel Buffer Attribute Keys for possible values.

`pixelBufferOut`  

On output, the newly created pixel buffer.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

Some of the parameters specified in this function override equivalent pixel buffer attributes. For example, if you set values for the kCVPixelBufferWidthKey and kCVPixelBufferHeightKey keys in the `pixelBufferAttributes` dictionary, the values for the `width` and `height` parameters override the values in the dictionary.

Use CVPixelBufferRelease to release ownership of the `pixelBufferOut` object when you’re done with it.

Tip

If you need to create and release multiple pixel buffers, use `CVPixelBufferPool` to create a pixel buffer pool that efficiently reuses pixel buffer memory.

## See Also

### Creating pixel buffers

func CVPixelBufferCreateWithBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer, Int, CVPixelBufferReleaseBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a pixel buffer for a given size and pixel format containing data specified by a memory location.

func CVPixelBufferCreateWithPlanarBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer?, Int, Int, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, CVPixelBufferReleasePlanarBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a single pixel buffer in planar format for a given size and pixel format containing data specified by a memory location.

func CVPixelBufferCreateWithIOSurface(CFAllocator?, IOSurfaceRef, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CVPixelBuffer>?>) -> CVReturn

Creates a single pixel buffer for the IO surface that you specify.

