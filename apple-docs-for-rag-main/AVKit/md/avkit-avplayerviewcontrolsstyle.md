

- AVKit
-  AVPlayerViewControlsStyle 

Enumeration

# AVPlayerViewControlsStyle

Constants that indicate which user interface controls the view displays.

macOS 10.9+

``` source
enum AVPlayerViewControlsStyle
```

## Topics

### Controls Styles

case none

The view displays no playback controls.

case inline

The view displays playback controls in a bar along the view’s bottom edge.

case floating

The view displays playback controls in a floating window over the video content.

case minimal

The view presents basic controls to play and pause playback.

static var `default`: AVPlayerViewControlsStyle

The view’s default controls style.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the User Interface

var controlsStyle: AVPlayerViewControlsStyle

The player view’s controls style.

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

