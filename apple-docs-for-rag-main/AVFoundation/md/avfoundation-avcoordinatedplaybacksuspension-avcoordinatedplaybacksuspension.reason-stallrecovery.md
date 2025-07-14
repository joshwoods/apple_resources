

- AVFoundation
- AVCoordinatedPlaybackSuspension
- AVCoordinatedPlaybackSuspension.Reason
-  stallRecovery 

Type Property

# stallRecovery

The player object is buffering media data after a stall.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static let stallRecovery: AVCoordinatedPlaybackSuspension.Reason
```

## See Also

### Suspension Reasons

static let audioSessionInterrupted: AVCoordinatedPlaybackSuspension.Reason

The system interrupts a participant’s audio session.

static let coordinatedPlaybackNotPossible: AVCoordinatedPlaybackSuspension.Reason

It’s not possible for a participant to start or resume coordinated playback.

static let playingInterstitial: AVCoordinatedPlaybackSuspension.Reason

A participant is playing content other than the primary content.

static let userActionRequired: AVCoordinatedPlaybackSuspension.Reason

A playback object requires user intervention to resume playback.

static let userIsChangingCurrentTime: AVCoordinatedPlaybackSuspension.Reason

A participant is actively changing the current time.

