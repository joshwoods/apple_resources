

- Core Video
-  CVPixelBufferCreateWithIOSurface(\_:\_:\_:\_:) 

Function

# CVPixelBufferCreateWithIOSurface(\_:\_:\_:\_:)

Creates a single pixel buffer for the IO surface that you specify.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func CVPixelBufferCreateWithIOSurface(
    _ allocator: CFAllocator?,
    _ surface: IOSurfaceRef,
    _ pixelBufferAttributes: CFDictionary?,
    _ pixelBufferOut: UnsafeMutablePointer?>
) -> CVReturn
```

## Parameters 

`allocator`  

The allocator to use for creating the buffer pool. Pass kCFAllocatorDefault for the `allocator` parameter to use the default allocator. See Predefined Allocators for additional values you can use.

`surface`  

The IOSurface to use in the pixel buffer.

`pixelBufferAttributes`  

An optional dictionary that contains the attributes for the pixel buffer. See Pixel Buffer Attribute Keys for possible values.

`pixelBufferOut`  

On output, the newly created pixel buffer.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

Use CVPixelBufferRelease to release ownership of the `pixelBufferOut` object when you’re done with it.

Important

If you are using IOSurface to share CVPixelBuffers between processes and those CVPixelBuffers are allocated via a CVPixelBufferPool, it is important that the CVPixelBufferPool does not reuse CVPixelBuffers whose IOSurfaces are still in use in other processes.

CoreVideo and IOSurface will take care of this for if you use IOSurfaceCreateMachPort and IOSurfaceLookupFromMachPort, but NOT if you pass IOSurfaceIDs.

## See Also

### Creating pixel buffers

func CVPixelBufferCreate(CFAllocator?, Int, Int, OSType, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a single pixel buffer for a given size and pixel format.

func CVPixelBufferCreateWithBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer, Int, CVPixelBufferReleaseBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a pixel buffer for a given size and pixel format containing data specified by a memory location.

func CVPixelBufferCreateWithPlanarBytes(CFAllocator?, Int, Int, OSType, UnsafeMutableRawPointer?, Int, Int, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, CVPixelBufferReleasePlanarBytesCallback?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a single pixel buffer in planar format for a given size and pixel format containing data specified by a memory location.

