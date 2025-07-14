

- AVKit
- AVPictureInPictureController
-  isPictureInPictureActive 

Instance Property

# isPictureInPictureActive

A Boolean value that indicates whether the Picture in Picture window is onscreen.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var isPictureInPictureActive: Bool { get }
```

## Discussion

This property is key-value observable.

## See Also

### Accessing Picture in Picture State

class func isPictureInPictureSupported() -> Bool

Returns a Boolean value that indicates whether the current device supports Picture in Picture.

var isPictureInPicturePossible: Bool

A Boolean value that indicates whether Picture in Picture playback is currently possible.

var isPictureInPictureSuspended: Bool

A Boolean value that indicates whether the system suspends the controller’s Picture in Picture window.

