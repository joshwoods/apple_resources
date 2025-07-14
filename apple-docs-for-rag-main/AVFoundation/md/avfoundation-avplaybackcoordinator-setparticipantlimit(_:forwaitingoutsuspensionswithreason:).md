

- AVFoundation
- AVPlaybackCoordinator
-  setParticipantLimit(\_:forWaitingOutSuspensionsWithReason:) 

Instance Method

# setParticipantLimit(\_:forWaitingOutSuspensionsWithReason:)

Sets a limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func setParticipantLimit(
    _ participantLimit: Int,
    forWaitingOutSuspensionsWithReason reason: AVCoordinatedPlaybackSuspension.Reason
)
```

## Parameters 

`participantLimit`  

The number of participants.

`reason`  

The suspension reason to set a limit for.

## Discussion

This method provides additional configuration of the values your app sets for the suspensionReasonsThatTriggerWaiting property. When a coordinator decides whether one participant’s suspensions cause others to wait, it also considers any participant limits that you set on the group.

## See Also

### Configuring Playback Policies

func participantLimitForWaitingOutSuspensions(withReason: AVCoordinatedPlaybackSuspension.Reason) -> Int

Returns the limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

var suspensionReasonsThatTriggerWaiting: [AVCoordinatedPlaybackSuspension.Reason]

The reasons that cause a coordinator to suspend playback.

var pauseSnapsToMediaTimeOfOriginator: Bool

A Boolean value that indicates whether participants mirror the originator’s stop time when they pause.

