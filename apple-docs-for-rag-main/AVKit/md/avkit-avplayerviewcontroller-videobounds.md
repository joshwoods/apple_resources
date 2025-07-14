

- AVKit
- AVPlayerViewController
-  videoBounds 

Instance Property

# videoBounds

The size and position of the video image within the bounds of the view controller’s view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var videoBounds: CGRect { get }
```

## Discussion

The size and position of this rectangle depend on the aspect ratio of the media (like 16:9 or 4:3), the bounds of the player view controller’s view, and the view controller’s videoGravity.

This property is key-value observable.

## See Also

### Configuring Presentation

var showsPlaybackControls: Bool

A Boolean value that indicates whether the player view controller shows playback controls.

var contentOverlayView: UIView?

A view that displays between the video content and the playback controls.

var videoGravity: AVLayerVideoGravity

A string that specifies how the video displays within the bounds of the view controller’s view.

var showsTimecodes: Bool

A Boolean value that determines whether the player view displays timecodes, if available.

var appliesPreferredDisplayCriteriaAutomatically: Bool

A Boolean value that indicates whether the view controller automatically sets the screen’s display criteria to match that of the currently playing asset.

