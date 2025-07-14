

- AVKit
- AVPictureInPictureController
-  canStopPictureInPicture 

Instance Property

# canStopPictureInPicture

A Boolean value that indicates whether Picture in Picture is active and is able to stop.

tvOS 14.0+

``` source
var canStopPictureInPicture: Bool { get }
```

## Mentioned in 

Adopting Picture in Picture in a Custom Player

## Discussion

When this value is true, calling stopPictureInPicture() stops the active Picture in Picture session. Apps should update the state of UI that starts Picture in Picture when this property value changes.

Thie value is key-value observable.

## See Also

### Controlling Picture in Picture Playback

var canStartPictureInPictureAutomaticallyFromInline: Bool

A Boolean value that indicates whether Picture in Picture starts automatically when the controller embeds its content inline and the app transitions to the background.

func startPictureInPicture()

Starts Picture in Picture, if possible.

func stopPictureInPicture()

Stops Picture in Picture, if active.

