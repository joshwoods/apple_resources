

- AVFoundation
-  AVPlaybackCoordinator 

Class

# AVPlaybackCoordinator

An object that coordinates the playback of players in a connected group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVPlaybackCoordinator
```

## Overview

The framework provides two playback coordinator subclasses that manage different types of player objects:

- AVPlayerPlaybackCoordinator coordinates the state of AVPlayer objects. If your app uses AVPlayer, continue to use its standard interfaces to control playback. The coordinator intercepts changes to the player’s rate and time, and propagates them to other players in the group.

- AVDelegatingPlaybackCoordinator coordinates the state of custom player objects. If your app uses a custom player, such as one that renders media using AVSampleBufferDisplayLayer and AVSampleBufferAudioRenderer, use this object to coordinate group playback. Adopt the coordinator’s delegate protocol so that your player responds to the commands that the coordinator issues.

Note

Use the Group Activities framework to connect a playback coordinator to its peers.

## Topics

### Configuring Playback Policies

func participantLimitForWaitingOutSuspensions(withReason: AVCoordinatedPlaybackSuspension.Reason) -> Int

Returns the limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

func setParticipantLimit(Int, forWaitingOutSuspensionsWithReason: AVCoordinatedPlaybackSuspension.Reason)

Sets a limit on the number of partipants that a group may contain before the coordinator stops waiting on suspensions that occur for a particular reason.

var suspensionReasonsThatTriggerWaiting: [AVCoordinatedPlaybackSuspension.Reason]

The reasons that cause a coordinator to suspend playback.

var pauseSnapsToMediaTimeOfOriginator: Bool

A Boolean value that indicates whether participants mirror the originator’s stop time when they pause.

### Suspending State Coordination

func beginSuspension(for: AVCoordinatedPlaybackSuspension.Reason) -> AVCoordinatedPlaybackSuspension

Tells the coordinator to stop sending playback commands temporarily when the playback object disconnects from the group activity.

class AVCoordinatedPlaybackSuspension

An object that represents a temporary suspension of coordinated playback.

func expectedItemTime(atHostTime: CMTime) -> CMTime

Returns a time in the current item’s timeline that the coordinator expects to play at the specified host time.

### Observing Suspension Reasons

var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason]

The reasons a coordinator is currently unable to participate in a group playback activity.

class let suspensionReasonsDidChangeNotification: NSNotification.Name

A notification that the coordinator posts when its suspension reasons change.

### Observing Other Participants

var otherParticipants: [AVCoordinatedPlaybackParticipant]

The identifiers of the other participants in a group.

class AVCoordinatedPlaybackParticipant

An object that represents a participant in a coordinated playback session.

class let otherParticipantsDidChangeNotification: NSNotification.Name

A notification that the coordinator posts when its other participants change.

### Coordinating with Group Sessions

func coordinateWithSession&lt;T>(GroupSession&lt;T>)

Begins coordination of a player with a group session.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVDelegatingPlaybackCoordinator
- AVPlayerPlaybackCoordinator

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### SharePlay

Destination Video

Leverage SwiftUI to build an immersive media experience in a multiplatform app.

Supporting Coordinated Media Playback

Create synchronized media experiences that enable users to watch and listen across devices.

class AVPlayerPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of player objects in a connected group.

class AVDelegatingPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of custom player objects in a connected group.

