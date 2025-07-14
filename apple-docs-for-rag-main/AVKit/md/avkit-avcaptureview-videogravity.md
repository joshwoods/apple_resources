

- AVKit
- AVCaptureView
-  videoGravity 

Instance Property

# videoGravity

A string value that defines how the capture view displays video within its bounds.

macOS 10.10+

``` source
@MainActor
var videoGravity: AVLayerVideoGravity { get set }
```

## Discussion

See AVLayerVideoGravity for supported values. The default value is resizeAspect.

## See Also

### Customizing the View

var controlsStyle: AVCaptureViewControlsStyle

The style of the capture controls presented by the view.

enum AVCaptureViewControlsStyle

Constants that describe the capture view’s supported controls styles.

