

- AVFoundation
- AVPlayerItem
-  customVideoCompositor 

Instance Property

# customVideoCompositor

The custom video compositor.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
nonisolated
var customVideoCompositor: (any AVVideoCompositing)? { get }
```

## Discussion

The custom video compositor instance that is used during image generation is accessible via this property after the value of videoComposition is set to an AVVideoComposition instance that specifies a custom video compositor class. Any additional communication between the application and that instance of the custom video compositor, if any is required for configuration or other purposes, can only occur once that has happened.

If the value of videoComposition is changed from an AVVideoComposition that specifies a custom video compositor class to another instance of AVVideoComposition that specifies the same custom video compositor class, the instance of the custom video compositor that was previously created will receive the renderContextChanged(_:) message and remain in use for subsequent image generation.

This property is `nil` if there is no video compositor, or if the internal video compositor is in use.

## See Also

### Configuring Video Compositing

var videoComposition: AVVideoComposition?

The video composition settings to be applied during playback.

var seekingWaitsForVideoCompositionRendering: Bool

A Boolean value that indicates whether the item’s timing follows the displayed video frame when seeking with a video composition.

