

- AVFoundation
- AVPlayer
- AVPlayer.RateDidChangeReason
-  setRateCalled 

Type Property

# setRateCalled

An app makes a call to set the player’s rate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static let setRateCalled: AVPlayer.RateDidChangeReason
```

## See Also

### Rate Change Reasons

static let appBackgrounded: AVPlayer.RateDidChangeReason

An app transitions to the background.

static let audioSessionInterrupted: AVPlayer.RateDidChangeReason

The system interrupts the app’s audio session.

static let setRateFailed: AVPlayer.RateDidChangeReason

An attempt to change the player’s rate fails.

