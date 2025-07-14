

- AVFoundation
- AVVideoCompositing
-  anticipateRendering(using:) 

Instance Method

# anticipateRendering(using:)

Informs a custom video compositor about upcoming rendering requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
optional func anticipateRendering(using renderHint: AVVideoCompositionRenderHint)
```

## Parameters 

`renderHint`  

Information about the upcoming composition requests.

## Discussion

In this method, the compositor can load composition resources, such as overlay images, that will be needed in the anticipated rendering time range.

Unlike the startRequest(_:) method, which is invoked only when the frame compositing is necessary, this method is typically called every frame duration. It allows the custom compositor to load and unload a composition resource such as overlay images at an appropriate time.

In forward playback, the render hint’s startCompositionTime is less than its endCompositionTime. In reverse playback, its endCompositionTime is less than its startCompositionTime. For seeking, the two values are equivalent, which means the upcoming composition request time range is unknown.

This method is guaranteed to be called before startRequest(_:) for a given composition time.

This method is synchronous. Make sure that your implementation returns quickly to ensure that playback doesn’t stall and cause frame drops.

## See Also

### Preparing to Render Frames

func prerollForRendering(using: AVVideoCompositionRenderHint)

Tells a custom video compositor to perform any work in the prerolling phase.

class AVVideoCompositionRenderHint

Information about upcoming composition requests, such as composition start time and end time.

