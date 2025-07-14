

- Core Video
-  CVPixelBufferCreateWithPlanarBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CVPixelBufferCreateWithPlanarBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a single pixel buffer in planar format for a given size and pixel format containing data specified by a memory location.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferCreateWithPlanarBytes(
    _ allocator: CFAllocator?,
    _ width: Int,
    _ height: Int,
    _ pixelFormatType: OSType,
    _ dataPtr: UnsafeMutableRawPointer?,
    _ dataSize: Int,
    _ numberOfPlanes: Int,
    _ planeBaseAddress: UnsafeMutablePointer,
    _ planeWidth: UnsafeMutablePointer,
    _ planeHeight: UnsafeMutablePointer,
    _ planeBytesPerRow: UnsafeMutablePointer,
    _ releaseCallback: CVPixelBufferReleasePlanarBytesCallback?,
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

The pixel format identified by its respective four-character code (type `OSType`).

`dataPtr`  

A pointer to a plane descriptor block if applicable, or `NULL` if it is not.

`dataSize`  

The size of the memory if the planes are contiguous, or `NULL` if it is not.

`numberOfPlanes`  

The number of planes.

`planeBaseAddress`  

The array of base addresses for the planes.

`planeWidth`  

The array of plane widths.

`planeHeight`  

The array of plane heights.

`planeBytesPerRow`  

The array of plane bytes-per-row values.

`releaseCallback`  

The callback function that gets called when the pixel buffer is destroyed. This callback allows the owner of the pixels to free the memory. See CVPixelBufferReleaseBytesCallback for more information.

`releaseRefCon`  

A pointer to user data identifying the pixel buffer. This value is passed to your pixel buffer release callback.

`pixelBufferAttributes`  

A dictionary with additional attributes for a a pixel buffer. This parameter is optional. See Pixel Buffer Attribute Keys for more details.

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

func CVPixelBufferCreateWithBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer, Int, CVPixelBufferReleaseBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a pixel buffer for a given size and pixel format containing data specified by a memory location.

func CVPixelBufferCreateWithIOSurface(CFAllocator?, IOSurfaceRef, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CVPixelBuffer>?>) -> CVReturn

Creates a single pixel buffer for the IO surface that you specify.

