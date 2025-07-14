

- AVFoundation
- AVPlayer
- AVPlayer.TimeControlStatus
-  AVPlayer.TimeControlStatus.paused 

Case

# AVPlayer.TimeControlStatus.paused

A state that indicates the player paused playback indefinitely.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case paused
```

## Discussion

In this state, the player pauses indefinitely and doesn’t resume playback until you call its play method. You can also resume playback if the player has sufficent data to start playback by calling the player’s setRate(_:time:atHostTime:) or playImmediately(atRate:) method with a nonzero rate value.

## See Also

### Status Values

case waitingToPlayAtSpecifiedRate

A state that indicates that the player is waiting for network conditions to improve before it can start or resume playback.

case playing

A state that indicates that the player is currently playing media.

