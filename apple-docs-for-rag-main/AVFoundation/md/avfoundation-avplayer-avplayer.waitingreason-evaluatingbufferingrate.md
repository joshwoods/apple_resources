

- AVFoundation
- AVPlayer
- AVPlayer.WaitingReason
-  evaluatingBufferingRate 

Type Property

# evaluatingBufferingRate

The player is waiting because it’s monitoring the buffer’s fill rate to determine whether playback is likely to complete without interruptions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let evaluatingBufferingRate: AVPlayer.WaitingReason
```

## See Also

### Player Waiting Reasons

static let noItemToPlay: AVPlayer.WaitingReason

The player is waiting because there’s no item to play.

static let toMinimizeStalls: AVPlayer.WaitingReason

The player is waiting for appropriate playback conditions before starting playback.

static let interstitialEvent: AVPlayer.WaitingReason

The player is waiting for an interstitial event to complete.

static let waitingForCoordinatedPlayback: AVPlayer.WaitingReason

The player is waiting for another participant in a coordinated playback session.

