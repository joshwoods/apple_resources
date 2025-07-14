

- AVKit
- AVPictureInPictureController
-  stopPictureInPicture() 

Instance Method

# stopPictureInPicture()

Stops Picture in Picture, if active.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func stopPictureInPicture()
```

## Discussion

Regardless of how Picture in Picture stops, the controller calls the delegate’s pictureInPictureControllerWillStopPictureInPicture(_:) method. When the PiP animation completes, the controller finalizes the session by calling the delegate’s pictureInPictureControllerDidStopPictureInPicture(_:) method.

## See Also

### Controlling Picture in Picture Playback

var canStopPictureInPicture: Bool

A Boolean value that indicates whether Picture in Picture is active and is able to stop.

var canStartPictureInPictureAutomaticallyFromInline: Bool

A Boolean value that indicates whether Picture in Picture starts automatically when the controller embeds its content inline and the app transitions to the background.

func startPictureInPicture()

Starts Picture in Picture, if possible.

