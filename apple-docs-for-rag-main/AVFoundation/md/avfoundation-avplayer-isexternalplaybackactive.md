

- AVFoundation
- AVPlayer
-  isExternalPlaybackActive 

Instance Property

# isExternalPlaybackActive

A Boolean value that indicates whether the player is currently playing video in external playback mode.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+

``` source
nonisolated
var isExternalPlaybackActive: Bool { get }
```

## See Also

### Managing External Playback

var allowsExternalPlayback: Bool

A Boolean value that indicates whether the player allows switching to external playback mode.

var usesExternalPlaybackWhileExternalScreenIsActive: Bool

A Boolean value that indicates whether the player should automatically switch to external playback mode while the external screen mode is active.

var externalPlaybackVideoGravity: AVLayerVideoGravity

The video gravity of the player for external playback mode only.

