

- Core Video
-  CVPixelBufferPoolFlush(\_:\_:) 

Function

# CVPixelBufferPoolFlush(\_:\_:)

Frees pixel buffers from the pool based on the options that you specify.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
func CVPixelBufferPoolFlush(
    _ pool: CVPixelBufferPool,
    _ options: CVPixelBufferPoolFlushFlags
)
```

## Parameters 

`pool`  

The pixel buffer pool to free.

`options`  

Set to excessBuffers to free all unused buffers regardless of their age. Pass an empty set to free only all aged-out buffers, or set it to excessBuffers to free all unused buffers regardless of age.

