

- AVFoundation
- AVPlaybackCoordinator
-  suspensionReasonsThatTriggerWaiting 

Instance Property

# suspensionReasonsThatTriggerWaiting

The reasons that cause a coordinator to suspend playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var suspensionReasonsThatTriggerWaiting: [AVCoordinatedPlaybackSuspension.Reason] { get set }
```

## See Also

### Configuring Playback Policies

func participantLimitForWaitingOutSuspensions(withReason: AVCoordinatedPlaybackSuspension.Reason) -> Int

Returns the limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

func setParticipantLimit(Int, forWaitingOutSuspensionsWithReason: AVCoordinatedPlaybackSuspension.Reason)

Sets a limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

var pauseSnapsToMediaTimeOfOriginator: Bool

A Boolean value that indicates whether participants mirror the originator’s stop time when they pause.

