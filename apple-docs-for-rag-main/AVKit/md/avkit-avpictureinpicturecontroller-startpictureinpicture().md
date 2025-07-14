

- AVKit
- AVPictureInPictureController
-  startPictureInPicture() 

Instance Method

# startPictureInPicture()

Starts Picture in Picture, if possible.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func startPictureInPicture()
```

## Mentioned in 

Adopting Picture in Picture for video calls

## Discussion

When you call this method and Picture in Picture (PiP) is possible, your delegate receives a call to its pictureInPictureControllerWillStartPictureInPicture(_:) method. After a successful start, your delegate receives a call to the pictureInPictureControllerDidStartPictureInPicture(_:) method.

If PiP fails, your delegate receives a call to the pictureInPictureController(_:failedToStartPictureInPictureWithError:)method.

Whether you explicitly stop PiP, the user stops it through interaction, or the system stops it, your delegate receives a call to the pictureInPictureControllerWillStopPictureInPicture(_:) method, followed by the pictureInPictureControllerDidStopPictureInPicture(_:) method after the PiP stop animation completes.

## See Also

### Controlling Picture in Picture Playback

var canStopPictureInPicture: Bool

A Boolean value that indicates whether Picture in Picture is active and is able to stop.

var canStartPictureInPictureAutomaticallyFromInline: Bool

A Boolean value that indicates whether Picture in Picture starts automatically when the controller embeds its content inline and the app transitions to the background.

func stopPictureInPicture()

Stops Picture in Picture, if active.

