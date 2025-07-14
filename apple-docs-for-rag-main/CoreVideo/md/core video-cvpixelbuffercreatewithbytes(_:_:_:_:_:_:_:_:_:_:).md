

- Core Video
-  CVPixelBufferCreateWithBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CVPixelBufferCreateWithBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a pixel buffer for a given size and pixel format containing data specified by a memory location.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferCreateWithBytes(
    _ allocator: CFAllocator?,
    _ width: Int,
    _ height: Int,
    _ pixelFormatType: OSType,
    _ baseAddress: UnsafeMutableRawPointer,
    _ bytesPerRow: Int,
    _ releaseCallback: CVPixelBufferReleaseBytesCallback?,
    _ releaseRefCon: UnsafeMutableRawPointer?,
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

The pixel format identified by its respective four character code (type `OSType`).

`baseAddress`  

A pointer to the base address of the memory storing the pixels.

`bytesPerRow`  

The row bytes of the pixel storage memory.

`releaseCallback`  

The callback function to be called when the pixel buffer is destroyed. This callback allows the owner of the pixels to free the memory. See CVPixelBufferReleaseBytesCallback for more information.

`releaseRefCon`  

The user data identifying the pixel buffer. This value is passed to your pixel buffer release callback.

`pixelBufferAttributes`  

A Core Foundation dictionary with additional attributes for a pixel buffer. This parameter is optional. See Pixel Buffer Attribute Keys for more details.

`pixelBufferOut`  

On output, the newly created pixel buffer. Ownership follows the The Create Rule.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

Some of the parameters specified in this call override equivalent pixel buffer attributes. For example, if you define the `kCVPixelBufferWidth` and `kCVPixelBufferHeight` keys in the pixel buffer attributes parameter (`pixelBufferAttributes`), these values are overridden by the `width` and `height` parameters.

## See Also

### Creating pixel buffers

func CVPixelBufferCreate(CFAllocator?, Int, Int, OSType, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a single pixel buffer for a given size and pixel format.

func CVPixelBufferCreateWithPlanarBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer?, Int, Int, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, CVPixelBufferReleasePlanarBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a single pixel buffer in planar format for a given size and pixel format containing data specified by a memory location.

func CVPixelBufferCreateWithIOSurface(CFAllocator?, IOSurfaceRef, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CVPixelBuffer>?>) -> CVReturn

Creates a single pixel buffer for the IO surface that you specify.

