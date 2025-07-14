

- AVFoundation
- AVPlayer
- AVPlayer.TimeControlStatus
-  AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate 

Case

# AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate

A state that indicates that the player is waiting for network conditions to improve before it can start or resume playback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case waitingToPlayAtSpecifiedRate
```

## Discussion

The player enters this state in the following conditions:

- Playback stalls because the playback buffer is empty.

- The playback rate changes from zero to a nonzero value and there isn’t enough media to start playback.

- The value of its currentItem property is `nil`.

In this state, the value of the rate property doesn’t indicate the current playback rate, but the rate at which playback starts or resumes. Refer to the value of reasonForWaitingToPlay for details about the player is waiting and the conditions that allow its status to change to AVPlayer.TimeControlStatus.playing.

Tip

While waiting for buffering, you can attempt to start playback of any available media data by calling playImmediately(atRate:).

## See Also

### Status Values

case paused

A state that indicates the player paused playback indefinitely.

case playing

A state that indicates that the player is currently playing media.

