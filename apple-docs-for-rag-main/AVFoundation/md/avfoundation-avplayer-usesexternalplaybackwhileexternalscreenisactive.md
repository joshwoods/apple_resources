

- AVFoundation
- AVPlayer
-  usesExternalPlaybackWhileExternalScreenIsActive 

Instance Property

# usesExternalPlaybackWhileExternalScreenIsActive

A Boolean value that indicates whether the player should automatically switch to external playback mode while the external screen mode is active.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+

``` source
nonisolated
var usesExternalPlaybackWhileExternalScreenIsActive: Bool { get set }
```

## Discussion

The player automatically switches back to the external screen mode once video playback concludes. A brief transition may be visible on the external display when automatically switching between the two modes. The default value of this property is false. The value of this property has no effect if allowsExternalPlayback is false.

## See Also

### Managing External Playback

var allowsExternalPlayback: Bool

A Boolean value that indicates whether the player allows switching to external playback mode.

var isExternalPlaybackActive: Bool

A Boolean value that indicates whether the player is currently playing video in external playback mode.

var externalPlaybackVideoGravity: AVLayerVideoGravity

The video gravity of the player for external playback mode only.

