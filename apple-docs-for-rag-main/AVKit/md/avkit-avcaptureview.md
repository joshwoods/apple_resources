

- AVKit
-  AVCaptureView 

Class

# AVCaptureView

A view that displays standard user interface controls for capturing media data.

macOS 10.10+

``` source
@MainActor
class AVCaptureView
```

## Topics

### Configuring the Capture Session

var session: AVCaptureSession?

The view’s associated capture session.

func setSession(AVCaptureSession?, showVideoPreview: Bool, showAudioPreview: Bool)

Sets the view’s capture session.

### Customizing the View

var controlsStyle: AVCaptureViewControlsStyle

The style of the capture controls presented by the view.

enum AVCaptureViewControlsStyle

Constants that describe the capture view’s supported controls styles.

var videoGravity: AVLayerVideoGravity

A string value that defines how the capture view displays video within its bounds.

### Configuring the Delegate

var delegate: (any AVCaptureViewDelegate)?

The capture view’s delegate object.

protocol AVCaptureViewDelegate

The protocol that defines the methods you can implement to respond to capture view events.

### Recording Media

var fileOutput: AVCaptureFileOutput?

The capture file output used to record media data.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### macOS Playback and Capture

Implementing Trimming in a macOS Player

Provide a QuickTime media-trimming experience in your macOS app.

class AVPlayerView

A view that displays content from a player and presents a native user interface to control playback.

