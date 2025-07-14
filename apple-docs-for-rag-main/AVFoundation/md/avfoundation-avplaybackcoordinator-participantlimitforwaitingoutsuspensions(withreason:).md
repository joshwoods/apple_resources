

- AVFoundation
- AVPlaybackCoordinator
-  participantLimitForWaitingOutSuspensions(withReason:) 

Instance Method

# participantLimitForWaitingOutSuspensions(withReason:)

Returns the limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func participantLimitForWaitingOutSuspensions(withReason reason: AVCoordinatedPlaybackSuspension.Reason) -> Int
```

## Parameters 

`reason`  

The suspension reason to find a participant limit for.

## Return Value

The participant limit.

## See Also

### Configuring Playback Policies

func setParticipantLimit(Int, forWaitingOutSuspensionsWithReason: AVCoordinatedPlaybackSuspension.Reason)

Sets a limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

var suspensionReasonsThatTriggerWaiting: [AVCoordinatedPlaybackSuspension.Reason]

The reasons that cause a coordinator to suspend playback.

var pauseSnapsToMediaTimeOfOriginator: Bool

A Boolean value that indicates whether participants mirror the originator’s stop time when they pause.

