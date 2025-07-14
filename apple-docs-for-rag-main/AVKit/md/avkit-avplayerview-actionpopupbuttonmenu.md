

- AVKit
- AVPlayerView
-  actionPopUpButtonMenu 

Instance Property

# actionPopUpButtonMenu

An action pop-up button menu that the player view displays.

macOS 10.9+

``` source
@IBOutlet @MainActor
var actionPopUpButtonMenu: NSMenu? { get set }
```

## Discussion

Set this property value to show an action pop-up button. Setting a custom action pop-up button is currently supported only for a controlsStyle of AVPlayerViewControlsStyle.floating or AVPlayerViewControlsStyle.inline.

The default value is `nil`.

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

var updatesNowPlayingInfoCenter: Bool

A Boolean value that indicates whether the player view controller updates the Now Playing info center.

