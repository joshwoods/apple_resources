

- AVKit
- AVPlayerView
-  isReadyForDisplay 

Instance Property

# isReadyForDisplay

A Boolean value that indicates whether the current player item’s first video frame is ready for display.

macOS 10.10+

``` source
@MainActor
var isReadyForDisplay: Bool { get }
```

## Discussion

This property value is key-value observable.

## See Also

### Customizing the Video Presentation

var videoBounds: NSRect

The current size and position of the video image that displays within the player view’s bounds.

var videoGravity: AVLayerVideoGravity

A value that determines how the player view displays video content within its bounds.

