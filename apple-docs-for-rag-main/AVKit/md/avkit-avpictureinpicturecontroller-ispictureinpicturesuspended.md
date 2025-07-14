

- AVKit
- AVPictureInPictureController
-  isPictureInPictureSuspended 

Instance Property

# isPictureInPictureSuspended

A Boolean value that indicates whether the system suspends the controller’s Picture in Picture window.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var isPictureInPictureSuspended: Bool { get }
```

## Discussion

The system suspends your app’s Picture in Picture session when another app, typically FaceTime, is using the feature. In this state, your video playback is active but paused and offscreen. Picture in Picture resumes automatically when the other app finishes using PiP.

## See Also

### Accessing Picture in Picture State

class func isPictureInPictureSupported() -> Bool

Returns a Boolean value that indicates whether the current device supports Picture in Picture.

var isPictureInPicturePossible: Bool

A Boolean value that indicates whether Picture in Picture playback is currently possible.

var isPictureInPictureActive: Bool

A Boolean value that indicates whether the Picture in Picture window is onscreen.

