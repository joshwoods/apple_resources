

- Core Video
-  CVPixelBufferPoolGetPixelBufferAttributes(\_:) 

Function

# CVPixelBufferPoolGetPixelBufferAttributes(\_:)

The attributes of pixel buffers which the system creates using the pool you specify.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolGetPixelBufferAttributes(_ pool: CVPixelBufferPool) -> CFDictionary?
```

## Parameters 

`pool`  

The pixel buffer pool that contains the attributes to retrieve.

## Return Value

A Core Foundation dictionary containing the pool attributes, or nil if the function fails.

## Discussion

Use this function to obtain information about the pixel buffers which the system creates using the pool you specify, before the system creates those pixel buffers.

## See Also

### Inspecting pools

func CVPixelBufferPoolGetAttributes(CVPixelBufferPool) -> CFDictionary?

The pool attributes dictionary for a pixel buffer pool.

func CVPixelBufferPoolGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the pixel buffer pool type.

