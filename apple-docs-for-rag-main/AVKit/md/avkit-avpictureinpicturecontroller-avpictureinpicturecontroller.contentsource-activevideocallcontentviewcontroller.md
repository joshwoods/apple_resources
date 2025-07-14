

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  activeVideoCallContentViewController 

Instance Property

# activeVideoCallContentViewController

The view controller that presents the video call content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var activeVideoCallContentViewController: AVPictureInPictureVideoCallViewController { get }
```

## Discussion

This view controller may indicate a preferred content size which influences the aspect ratio and the size of the Picture in Picture window. The view it presents isn’t interactive and doesn’t receive touches or user input.

When this view controller’s appearance methods indicate that its view is on screen, place the video call content view in the controller’s view hierarchy. The content must fill the bounds of the view controller’s view.

Although apps can choose to move content from their source view to this view controller, it’s also valid to show different views, as long as they represent the same video call.

## See Also

### Accessing the Active Call Presentation

var activeVideoCallSourceView: UIView?

The view that contains the video content of the call.

class AVPictureInPictureVideoCallViewController

A view controller that presents content from a video call in Picture in Picture.

