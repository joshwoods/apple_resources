

- AVKit
- AVPlayerView
-  showsTimecodes 

Instance Property

# showsTimecodes

A Boolean value that determines whether the player view displays timecodes, if available.

macOS 10.15+

``` source
@MainActor
var showsTimecodes: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Customizing the User Interface

var controlsStyle: AVPlayerViewControlsStyle

The player view’s controls style.

enum AVPlayerViewControlsStyle

Constants that indicate which user interface controls the view displays.

var showsFrameSteppingButtons: Bool

A Boolean value that determines whether the player view displays frame stepping buttons.

var showsSharingServiceButton: Bool

A Boolean value that determines whether the player view displays a sharing service button.

var showsFullScreenToggleButton: Bool

A Boolean value that determines whether the player view displays a full-screen toggle button.

var contentOverlayView: NSView?

A view that adds additional custom views between the video content and the controls.

var actionPopUpButtonMenu: NSMenu?

An action pop-up button menu that the player view displays.

var updatesNowPlayingInfoCenter: Bool

A Boolean value that indicates whether the player view controller updates the Now Playing info center.

