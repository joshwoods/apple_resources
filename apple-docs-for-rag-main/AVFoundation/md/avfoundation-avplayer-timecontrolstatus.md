

- AVFoundation
- AVPlayer
-  timeControlStatus 

Instance Property

# timeControlStatus

A value that indicates whether playback is in progress, paused indefinitely, or waiting for network conditions to improve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
nonisolated
var timeControlStatus: AVPlayer.TimeControlStatus { get }
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

When the value of automaticallyWaitsToMinimizeStalling is true, the player waits until your app resumes playback.

During playback, the value of the property changes between AVPlayer.TimeControlStatus.playing and AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate depending on whether the player has sufficient media data to continue playback.

This property is key-value observable.

## See Also

### Configuring Waiting Behavior

var automaticallyWaitsToMinimizeStalling: Bool

A Boolean value that indicates whether the player should automatically delay playback in order to minimize stalling.

var reasonForWaitingToPlay: AVPlayer.WaitingReason?

The reason the player is currently waiting for playback to begin or resume.

struct WaitingReason

The reasons a player is waiting to begin or resume playback.

enum TimeControlStatus

Constants that indicate the state of playback control.

func playImmediately(atRate: Float)

Plays the available media data immediately, at the specified rate.

