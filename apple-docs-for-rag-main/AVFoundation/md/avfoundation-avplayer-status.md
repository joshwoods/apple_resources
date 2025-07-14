

- AVFoundation
- AVPlayer
-  status 

Instance Property

# status

A value that indicates the readiness of a player object for playback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var status: AVPlayer.Status { get }
```

## Discussion

If the value of this property is AVPlayer.Status.failed, check the value of the player’s error property to determine the nature of the failure. If a player reaches a failed state, you can’t use it for playback, and instead need to create a new instance.

This property is key-value observable.

Note

The player’s status doesn’t indicate its readiness to play a specific player item. You should instead use the status property of AVPlayerItem to make that determination.

## See Also

### Determining Player Readiness

enum Status

Status values that indicate whether a player can successfully play media.

var error: (any Error)?

An error that caused a failure.

