

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  activeVideoCallSourceView 

Instance Property

# activeVideoCallSourceView

The view that contains the video content of the call.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
weak var activeVideoCallSourceView: UIView? { get }
```

## Discussion

The controller uses this view’s layout frame and visibility to determine whether or not Picture in Picture begins automatically when the app moves to the background. The view’s layout frame also influences the animation when entering and exiting Picture in Picture.

## See Also

### Accessing the Active Call Presentation

var activeVideoCallContentViewController: AVPictureInPictureVideoCallViewController

The view controller that presents the video call content.

class AVPictureInPictureVideoCallViewController

A view controller that presents content from a video call in Picture in Picture.

