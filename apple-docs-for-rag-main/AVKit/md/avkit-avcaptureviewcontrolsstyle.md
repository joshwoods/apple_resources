

- AVKit
-  AVCaptureViewControlsStyle 

Enumeration

# AVCaptureViewControlsStyle

Constants that describe the capture view’s supported controls styles.

macOS 10.10+

``` source
enum AVCaptureViewControlsStyle
```

## Topics

### Controls Styles

case inline

The view’s inline controls style.

case floating

The view’s floating controls style, which matches the user interface of QuickTime Player.

case inlineDeviceSelection

The view’s inline device selection style.

static var `default`: AVCaptureViewControlsStyle

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

### Customizing the View

var controlsStyle: AVCaptureViewControlsStyle

The style of the capture controls presented by the view.

var videoGravity: AVLayerVideoGravity

A string value that defines how the capture view displays video within its bounds.

