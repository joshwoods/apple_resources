

- AVFoundation
- AVPlayer
-  AVPlayer.WaitingReason 

Structure

# AVPlayer.WaitingReason

The reasons a player is waiting to begin or resume playback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct WaitingReason
```

## Topics

### Player Waiting Reasons

static let evaluatingBufferingRate: AVPlayer.WaitingReason

The player is waiting because it’s monitoring the buffer’s fill rate to determine whether playback is likely to complete without interruptions.

static let noItemToPlay: AVPlayer.WaitingReason

The player is waiting because there’s no item to play.

static let toMinimizeStalls: AVPlayer.WaitingReason

The player is waiting for appropriate playback conditions before starting playback.

static let interstitialEvent: AVPlayer.WaitingReason

The player is waiting for an interstitial event to complete.

static let waitingForCoordinatedPlayback: AVPlayer.WaitingReason

The player is waiting for another participant in a coordinated playback session.

### Initializers

init(rawValue: String)

Creates a waiting reason with a string value.

## Relationships

### Conforms To

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

var timeControlStatus: AVPlayer.TimeControlStatus

A value that indicates whether playback is in progress, paused indefinitely, or waiting for network conditions to improve.

enum TimeControlStatus

Constants that indicate the state of playback control.

func playImmediately(atRate: Float)

Plays the available media data immediately, at the specified rate.

