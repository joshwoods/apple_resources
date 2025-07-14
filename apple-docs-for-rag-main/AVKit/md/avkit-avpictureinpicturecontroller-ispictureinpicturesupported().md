

- AVKit
- AVPictureInPictureController
-  isPictureInPictureSupported() 

Type Method

# isPictureInPictureSupported()

Returns a Boolean value that indicates whether the current device supports Picture in Picture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class func isPictureInPictureSupported() -> Bool
```

## Return Value

true if the current device supports Picture in Picture playback, otherwise false.

## Mentioned in 

Adopting Picture in Picture for video calls

Adopting Picture in Picture in a Custom Player

## Discussion

If Picture in Picture isn’t supported on the current device, attempting to initialize a Picture in Picture controller returns `nil`.

## See Also

### Accessing Picture in Picture State

var isPictureInPicturePossible: Bool

A Boolean value that indicates whether Picture in Picture playback is currently possible.

var isPictureInPictureActive: Bool

A Boolean value that indicates whether the Picture in Picture window is onscreen.

var isPictureInPictureSuspended: Bool

A Boolean value that indicates whether the system suspends the controller’s Picture in Picture window.

