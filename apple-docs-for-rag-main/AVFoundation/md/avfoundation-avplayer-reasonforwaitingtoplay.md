

- AVFoundation
- AVPlayer
-  reasonForWaitingToPlay 

Instance Property

# reasonForWaitingToPlay

The reason the player is currently waiting for playback to begin or resume.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
nonisolated
var reasonForWaitingToPlay: AVPlayer.WaitingReason? { get }
```

## Discussion

When the value of the player’s timeControlStatus is AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate, you can use this property determine the reason the player is currently waiting for playback to begin or resume. Possible values for this property are:

- toMinimizeStalls

- noItemToPlay

- evaluatingBufferingRate

The value of this property will be `nil` if the player’s timeControlStatus is a value other than AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate.

You can use the value of this property to conditionally show UI indicating the player’s waiting state. This property is observable using key-value observing.

## See Also

### Configuring Waiting Behavior

var automaticallyWaitsToMinimizeStalling: Bool

A Boolean value that indicates whether the player should automatically delay playback in order to minimize stalling.

struct WaitingReason

The reasons a player is waiting to begin or resume playback.

var timeControlStatus: AVPlayer.TimeControlStatus

A value that indicates whether playback is in progress, paused indefinitely, or waiting for network conditions to improve.

enum TimeControlStatus

Constants that indicate the state of playback control.

func playImmediately(atRate: Float)

Plays the available media data immediately, at the specified rate.

