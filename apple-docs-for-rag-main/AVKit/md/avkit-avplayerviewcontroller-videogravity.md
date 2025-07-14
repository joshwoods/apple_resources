

- AVKit
- AVPlayerViewController
-  videoGravity 

Instance Property

# videoGravity

A string that specifies how the video displays within the bounds of the view controller’s view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var videoGravity: AVLayerVideoGravity { get set }
```

## Discussion

The player view controller supports the following video gravity values: resizeAspect, resizeAspectFill, and resize.

The default value is resizeAspect.

## See Also

### Configuring Presentation

var showsPlaybackControls: Bool

A Boolean value that indicates whether the player view controller shows playback controls.

var contentOverlayView: UIView?

A view that displays between the video content and the playback controls.

var videoBounds: CGRect

The size and position of the video image within the bounds of the view controller’s view.

var showsTimecodes: Bool

A Boolean value that determines whether the player view displays timecodes, if available.

var appliesPreferredDisplayCriteriaAutomatically: Bool

A Boolean value that indicates whether the view controller automatically sets the screen’s display criteria to match that of the currently playing asset.

