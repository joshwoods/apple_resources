

- AVKit
- AVPlayerView
-  controlsStyle 

Instance Property

# controlsStyle

The player view’s controls style.

macOS 10.9+

``` source
@MainActor
var controlsStyle: AVPlayerViewControlsStyle { get set }
```

## Discussion

The player view supports several different control styles that you can use to customize the player view’s appearance and behavior. See AVPlayerViewControlsStyle for the possible values.

## See Also

### Customizing the User Interface

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

var updatesNowPlayingInfoCenter: Bool

A Boolean value that indicates whether the player view controller updates the Now Playing info center.

