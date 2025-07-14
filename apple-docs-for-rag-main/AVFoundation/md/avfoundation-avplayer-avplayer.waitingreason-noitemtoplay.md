

- AVFoundation
- AVPlayer
- AVPlayer.WaitingReason
-  noItemToPlay 

Type Property

# noItemToPlay

The player is waiting because there’s no item to play.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let noItemToPlay: AVPlayer.WaitingReason
```

## See Also

### Player Waiting Reasons

static let evaluatingBufferingRate: AVPlayer.WaitingReason

The player is waiting because it’s monitoring the buffer’s fill rate to determine whether playback is likely to complete without interruptions.

static let toMinimizeStalls: AVPlayer.WaitingReason

The player is waiting for appropriate playback conditions before starting playback.

static let interstitialEvent: AVPlayer.WaitingReason

The player is waiting for an interstitial event to complete.

static let waitingForCoordinatedPlayback: AVPlayer.WaitingReason

The player is waiting for another participant in a coordinated playback session.

