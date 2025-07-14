

- AVKit
- AVPlayerViewController
-  allowsPictureInPicturePlayback 

Instance Property

# allowsPictureInPicturePlayback

A Boolean value that indicates whether the player allows Picture in Picture playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var allowsPictureInPicturePlayback: Bool { get set }
```

## Discussion

Set this value to false to disable Picture in Picture playback. The default value is true.

## See Also

### Configuring Picture in Picture

var canStartPictureInPictureAutomaticallyFromInline: Bool

A Boolean value that indicates whether Picture in Picture starts automatically when transitioning to the background when the view controller presents its content inline.

