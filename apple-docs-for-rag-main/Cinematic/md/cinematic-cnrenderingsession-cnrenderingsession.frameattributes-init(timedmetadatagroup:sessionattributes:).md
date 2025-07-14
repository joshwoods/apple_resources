

- Cinematic
- CNRenderingSession
- CNRenderingSession.FrameAttributes
-  init(timedMetadataGroup:sessionAttributes:) 

Initializer

# init(timedMetadataGroup:sessionAttributes:)

Creates a structure representing a Cinematic rendering session based on meta group and session attributes.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init?(
    timedMetadataGroup metadataGroup: AVTimedMetadataGroup,
    sessionAttributes: CNRenderingSession.Attributes
)
```

## Parameters 

`metadataGroup`  

The meta group read from the timed Cinematic metadata track of a Cinematic asset.

`sessionAttributes`  

Rendering session attributes loaded from a Cinematic asset.

