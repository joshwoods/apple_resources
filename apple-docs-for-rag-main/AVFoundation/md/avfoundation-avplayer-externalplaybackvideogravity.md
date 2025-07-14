

- AVFoundation
- AVPlayer
-  externalPlaybackVideoGravity 

Instance Property

# externalPlaybackVideoGravity

The video gravity of the player for external playback mode only.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+

``` source
nonisolated
var externalPlaybackVideoGravity: AVLayerVideoGravity { get set }
```

## Discussion

Valid values are resize, resizeAspectFill, or resizeAspect.

## See Also

### Managing External Playback

var allowsExternalPlayback: Bool

A Boolean value that indicates whether the player allows switching to external playback mode.

var isExternalPlaybackActive: Bool

A Boolean value that indicates whether the player is currently playing video in external playback mode.

var usesExternalPlaybackWhileExternalScreenIsActive: Bool

A Boolean value that indicates whether the player should automatically switch to external playback mode while the external screen mode is active.

