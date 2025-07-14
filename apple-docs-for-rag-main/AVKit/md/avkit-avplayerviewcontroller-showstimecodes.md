

- AVKit
- AVPlayerViewController
-  showsTimecodes 

Instance Property

# showsTimecodes

A Boolean value that determines whether the player view displays timecodes, if available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var showsTimecodes: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Configuring Presentation

var showsPlaybackControls: Bool

A Boolean value that indicates whether the player view controller shows playback controls.

var contentOverlayView: UIView?

A view that displays between the video content and the playback controls.

var videoGravity: AVLayerVideoGravity

A string that specifies how the video displays within the bounds of the view controller’s view.

var videoBounds: CGRect

The size and position of the video image within the bounds of the view controller’s view.

var appliesPreferredDisplayCriteriaAutomatically: Bool

A Boolean value that indicates whether the view controller automatically sets the screen’s display criteria to match that of the currently playing asset.

