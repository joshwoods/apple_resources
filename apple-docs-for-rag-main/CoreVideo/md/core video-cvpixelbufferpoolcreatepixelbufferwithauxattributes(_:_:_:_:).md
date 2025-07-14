

- Core Video
-  CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(\_:\_:\_:\_:) 

Function

# CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(\_:\_:\_:\_:)

Creates a new pixel buffer with auxiliary attributes from the pool.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(
    _ allocator: CFAllocator?,
    _ pixelBufferPool: CVPixelBufferPool,
    _ auxAttributes: CFDictionary?,
    _ pixelBufferOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The allocator to use for creating the buffer pool. Pass kCFAllocatorDefault to use the default allocator. See Predefined Allocators for additional values you can use.

`pixelBufferPool`  

The pixel buffer pool for creating the new pixel buffer.

`auxAttributes`  

An optional dictionary of auxiliary attributes that describes the allocation request. See the Constants topic group below for possible values.

`pixelBufferOut`  

On output, the newly created pixel buffer.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

This function creates a new CVPixelBuffer object using the pixel buffer attributes specified during pool creation and the attributes specified in the `auxAttributes` parameter.

## See Also

### Creating pools

func CVPixelBufferPoolCreate(CFAllocator?, CFDictionary?, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBufferPool?>) -> CVReturn

Creates a pixel buffer pool using the allocator and attributes that you specify.

func CVPixelBufferPoolCreatePixelBuffer(CFAllocator?, CVPixelBufferPool, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a pixel buffer from a pixel buffer pool, using the allocator that you specify.

