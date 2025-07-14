

- Video Toolbox
- VTFrameProcessorOpticalFlow
-  init(forwardFlow:backwardFlow:) 

Initializer

# init(forwardFlow:backwardFlow:)

Creates an object with forward and backward optical flow pixel buffers.

macOS 15.4+

``` source
init?(
    forwardFlow: CVPixelBuffer,
    backwardFlow: CVPixelBuffer
)
```

## Parameters 

`forwardFlow`  

A pixel buffer that contains forward optical flow. This value must be non-NULL and IOSurface backed.

`backwardFlow`  

A pixel buffer that contains backward optical flow. his value must be non-NULL and IOSurface backed.

## Discussion

Instances retain the buffers backing them. Returns NULL if a NULL CVPixelBuffer is provided or if CVPixelBuffers are not IOSurface backed.

