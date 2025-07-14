

- AVKit
- AVPlayerView
-  videoBounds 

Instance Property

# videoBounds

The current size and position of the video image that displays within the player view’s bounds.

macOS 10.10+

``` source
@MainActor
var videoBounds: NSRect { get }
```

## Discussion

Use this property to determine the display dimensions of the video image within the player view’s bounds. The size and position of this rectangle depend on the aspect ratio of the media (like 16:9 or 4:3), the player view’s bounds, and its controlsStyle.

## See Also

### Customizing the Video Presentation

var isReadyForDisplay: Bool

A Boolean value that indicates whether the current player item’s first video frame is ready for display.

var videoGravity: AVLayerVideoGravity

A value that determines how the player view displays video content within its bounds.

