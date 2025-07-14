

- Core Video
-  CVPixelBufferPoolCreatePixelBuffer(\_:\_:\_:) 

Function

# CVPixelBufferPoolCreatePixelBuffer(\_:\_:\_:)

Creates a pixel buffer from a pixel buffer pool, using the allocator that you specify.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolCreatePixelBuffer(
    _ allocator: CFAllocator?,
    _ pixelBufferPool: CVPixelBufferPool,
    _ pixelBufferOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The allocator to use for creating the pixel buffer. Pass kCFAllocatorDefault to use the default allocator. See Predefined Allocators for additional values you can use.

`pixelBufferPool`  

The pixel buffer pool for creating the new pixel buffer.

`pixelBufferOut`  

On output, the newly created pixel buffer.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

This function creates a new pixel buffer using the pixel buffer attributes specified during pool creation. This buffer has default attachments as specified in the `pixelBufferAttributes` parameter of CVPixelBufferPoolCreate(_:_:_:_:), using either the kCVBufferPropagatedAttachmentsKey or kCVBufferNonPropagatedAttachmentsKey attributes.

## See Also

### Creating pools

func CVPixelBufferPoolCreate(CFAllocator?, CFDictionary?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBufferPool?>) -> CVReturn

Creates a pixel buffer pool using the allocator and attributes that you specify.

func CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(CFAllocator?, CVPixelBufferPool, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a new pixel buffer with auxiliary attributes from the pool.

