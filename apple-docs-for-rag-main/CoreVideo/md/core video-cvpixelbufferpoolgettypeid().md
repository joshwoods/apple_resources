

- Core Video
-  CVPixelBufferPoolGetTypeID() 

Function

# CVPixelBufferPoolGetTypeID()

Returns the Core Foundation type identifier of the pixel buffer pool type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferPoolGetTypeID() -> CFTypeID
```

## Return Value

The Core Foundation type identifier for this pixel buffer.

## See Also

### Inspecting pools

func CVPixelBufferPoolGetAttributes(CVPixelBufferPool) -> CFDictionary?

The pool attributes dictionary for a pixel buffer pool.

func CVPixelBufferPoolGetPixelBufferAttributes(CVPixelBufferPool) -> CFDictionary?

The attributes of pixel buffers which the system creates using the pool you specify.

