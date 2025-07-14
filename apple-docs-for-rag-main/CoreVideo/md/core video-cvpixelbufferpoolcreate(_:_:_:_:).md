

- Core Video
-  CVPixelBufferPoolCreate(\_:\_:\_:\_:) 

Function

# CVPixelBufferPoolCreate(\_:\_:\_:\_:)

Creates a pixel buffer pool using the allocator and attributes that you specify.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolCreate(
    _ allocator: CFAllocator?,
    _ poolAttributes: CFDictionary?,
    _ pixelBufferAttributes: CFDictionary?,
    _ poolOut: UnsafeMutablePointer
) -> CVReturn
```

## Parameters 

`allocator`  

The allocator to use for creating the buffer pool. Pass kCFAllocatorDefault to use the default allocator. See Predefined Allocators for additional values you can use.

`poolAttributes`  

A Core Foundation dictionary that contains the attributes for the pixel buffer pool. See the Constants topic group below for possible values.

`pixelBufferAttributes`  

An optional dictionary that contains the attributes to use to create new pixel buffers within the pool. See Pixel Buffer Attribute Keys for possible values.

`poolOut`  

On output, the newly created pixel buffer pool.

## Return Value

A Core Video result code. See Result Codes for possible values.

## Discussion

Use CVPixelBufferPoolRelease to release ownership of the `poolOut` object when you’re done with it.

## See Also

### Creating pools

func CVPixelBufferPoolCreatePixelBuffer(CFAllocator?, CVPixelBufferPool, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a pixel buffer from a pixel buffer pool, using the allocator that you specify.

func CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(CFAllocator?, CVPixelBufferPool, CFDictionary?, UnsafeMutablePointer&lt;CVPixelBuffer?>) -> CVReturn

Creates a new pixel buffer with auxiliary attributes from the pool.

