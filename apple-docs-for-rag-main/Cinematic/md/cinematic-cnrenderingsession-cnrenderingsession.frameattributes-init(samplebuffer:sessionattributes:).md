

- Cinematic
- CNRenderingSession
- CNRenderingSession.FrameAttributes
-  init(sampleBuffer:sessionAttributes:) 

Initializer

# init(sampleBuffer:sessionAttributes:)

Creates a structure representing a Cinematic rendering session based a sample buffer and session attributes.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init?(
    sampleBuffer: CMSampleBuffer,
    sessionAttributes: CNRenderingSession.Attributes
)
```

## Parameters 

`sampleBuffer`  

A sample buffer read from the timed Cinematic metadata track of a cinematic asset.

`sessionAttributes`  

Rendering session attributes loaded from a Cinematic asset.

