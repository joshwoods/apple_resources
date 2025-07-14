

- AVKit
- AVPictureInPictureController
-  isPictureInPicturePossible 

Instance Property

# isPictureInPicturePossible

A Boolean value that indicates whether Picture in Picture playback is currently possible.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var isPictureInPicturePossible: Bool { get }
```

## Mentioned in 

Adopting Picture in Picture in a Custom Player

## Discussion

This property value is false if another app, like FaceTime, is presenting Picture in Picture content.

This property is key-value observable.

## See Also

### Accessing Picture in Picture State

class func isPictureInPictureSupported() -> Bool

Returns a Boolean value that indicates whether the current device supports Picture in Picture.

var isPictureInPictureActive: Bool

A Boolean value that indicates whether the Picture in Picture window is onscreen.

var isPictureInPictureSuspended: Bool

A Boolean value that indicates whether the system suspends the controller’s Picture in Picture window.

