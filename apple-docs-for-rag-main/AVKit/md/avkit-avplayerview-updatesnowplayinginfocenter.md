

- AVKit
- AVPlayerView
-  updatesNowPlayingInfoCenter 

Instance Property

# updatesNowPlayingInfoCenter

A Boolean value that indicates whether the player view controller updates the Now Playing info center.

macOS 10.13+

``` source
@MainActor
var updatesNowPlayingInfoCenter: Bool { get set }
```

## Discussion

The default value is true.

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

var showsTimecodes: Bool

A Boolean value that determines whether the player view displays timecodes, if available.

var contentOverlayView: NSView?

A view that adds additional custom views between the video content and the controls.

var actionPopUpButtonMenu: NSMenu?

An action pop-up button menu that the player view displays.

