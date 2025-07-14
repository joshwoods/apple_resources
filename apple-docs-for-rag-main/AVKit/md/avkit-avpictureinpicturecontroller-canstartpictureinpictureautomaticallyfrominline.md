

- AVKit
- AVPictureInPictureController
-  canStartPictureInPictureAutomaticallyFromInline 

Instance Property

# canStartPictureInPictureAutomaticallyFromInline

A Boolean value that indicates whether Picture in Picture starts automatically when the controller embeds its content inline and the app transitions to the background.

iOS 14.2+iPadOS 14.2+Mac Catalyst 14.2+visionOS 1.0+

``` source
var canStartPictureInPictureAutomaticallyFromInline: Bool { get set }
```

## Mentioned in 

Adopting Picture in Picture for video calls

## Discussion

Only set this value to true for content that you intend to be the user’s primary focus.

## See Also

### Controlling Picture in Picture Playback

var canStopPictureInPicture: Bool

A Boolean value that indicates whether Picture in Picture is active and is able to stop.

func startPictureInPicture()

Starts Picture in Picture, if possible.

func stopPictureInPicture()

Stops Picture in Picture, if active.

