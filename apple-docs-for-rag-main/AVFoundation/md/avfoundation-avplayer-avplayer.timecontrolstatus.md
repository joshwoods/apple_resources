

- AVFoundation
- AVPlayer
-  AVPlayer.TimeControlStatus 

Enumeration

# AVPlayer.TimeControlStatus

Constants that indicate the state of playback control.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum TimeControlStatus
```

## Topics

### Status Values

case paused

A state that indicates the player paused playback indefinitely.

case waitingToPlayAtSpecifiedRate

A state that indicates that the player is waiting for network conditions to improve before it can start or resume playback.

case playing

A state that indicates that the player is currently playing media.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Waiting Behavior

var automaticallyWaitsToMinimizeStalling: Bool

A Boolean value that indicates whether the player should automatically delay playback in order to minimize stalling.

var reasonForWaitingToPlay: AVPlayer.WaitingReason?

The reason the player is currently waiting for playback to begin or resume.

struct WaitingReason

The reasons a player is waiting to begin or resume playback.

var timeControlStatus: AVPlayer.TimeControlStatus

A value that indicates whether playback is in progress, paused indefinitely, or waiting for network conditions to improve.

func playImmediately(atRate: Float)

Plays the available media data immediately, at the specified rate.

