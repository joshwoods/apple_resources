

- Core Video
-  CVPixelBufferPoolGetAttributes(\_:) 

Function

# CVPixelBufferPoolGetAttributes(\_:)

The pool attributes dictionary for a pixel buffer pool.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolGetAttributes(_ pool: CVPixelBufferPool) -> CFDictionary?
```

## Parameters 

`pool`  

The pixel buffer pool that contains the attributes to retrieve.

## Return Value

A Core Foundation dictionary containing the pool attributes, or nil if the function fails.

## See Also

### Inspecting pools

func CVPixelBufferPoolGetPixelBufferAttributes(CVPixelBufferPool) -> CFDictionary?

The attributes of pixel buffers which the system creates using the pool you specify.

func CVPixelBufferPoolGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the pixel buffer pool type.

