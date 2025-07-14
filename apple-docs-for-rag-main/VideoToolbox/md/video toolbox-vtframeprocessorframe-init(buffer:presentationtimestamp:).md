

- Video Toolbox
- VTFrameProcessorFrame
-  init(buffer:presentationTimeStamp:) 

Initializer

# init(buffer:presentationTimeStamp:)

Creates a frame object with a pixel buffer and presentation time.

macOS 15.4+

``` source
init?(
    buffer: CVPixelBuffer,
    presentationTimeStamp: CMTime
)
```

## Parameters 

`buffer`  

A pixel buffer for the frame. This value must be non-NULL and IOSurface backed.

`presentationTimeStamp`  

The presentation timestamp of the buffer.

## Discussion

Initialization fails if you specify a `NULL` buffer or one that isn’t backed by an `IOSurface`.

