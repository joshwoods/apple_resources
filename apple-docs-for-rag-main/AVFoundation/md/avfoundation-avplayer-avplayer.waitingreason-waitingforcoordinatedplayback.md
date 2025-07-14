

- AVFoundation
- AVPlayer
- AVPlayer.WaitingReason
-  waitingForCoordinatedPlayback 

Type Property

# waitingForCoordinatedPlayback

The player is waiting for another participant in a coordinated playback session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static let waitingForCoordinatedPlayback: AVPlayer.WaitingReason
```

## See Also

### Player Waiting Reasons

static let evaluatingBufferingRate: AVPlayer.WaitingReason

The player is waiting because it’s monitoring the buffer’s fill rate to determine whether playback is likely to complete without interruptions.

static let noItemToPlay: AVPlayer.WaitingReason

The player is waiting because there’s no item to play.

static let toMinimizeStalls: AVPlayer.WaitingReason

The player is waiting for appropriate playback conditions before starting playback.

static let interstitialEvent: AVPlayer.WaitingReason

The player is waiting for an interstitial event to complete.

