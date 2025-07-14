

- AVFoundation
- AVPlayer
-  allowsExternalPlayback 

Instance Property

# allowsExternalPlayback

A Boolean value that indicates whether the player allows switching to external playback mode.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+

``` source
nonisolated
var allowsExternalPlayback: Bool { get set }
```

## Discussion

The default value of this property is true.

## See Also

### Managing External Playback

var isExternalPlaybackActive: Bool

A Boolean value that indicates whether the player is currently playing video in external playback mode.

var usesExternalPlaybackWhileExternalScreenIsActive: Bool

A Boolean value that indicates whether the player should automatically switch to external playback mode while the external screen mode is active.

var externalPlaybackVideoGravity: AVLayerVideoGravity

The video gravity of the player for external playback mode only.

