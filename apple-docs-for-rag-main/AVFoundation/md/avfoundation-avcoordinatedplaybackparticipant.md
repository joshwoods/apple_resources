

- AVFoundation
-  AVCoordinatedPlaybackParticipant 

Class

# AVCoordinatedPlaybackParticipant

An object that represents a participant in a coordinated playback session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVCoordinatedPlaybackParticipant
```

## Overview

Access the other participants in a session through the playback coordinator’s otherParticipants property to determine their playback readiness and suspension reasons.

## Topics

### Accessing Participant Status

var identifier: UUID

A unique identifier for the participant.

var isReadyToPlay: Bool

A Boolean value that indicates whether the participant is ready to start coordinated playback.

var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason]

The reasons a participant isn’t currently participating in coordinated playback.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Observing Other Participants

var otherParticipants: [AVCoordinatedPlaybackParticipant]

The identifiers of the other participants in a group.

class let otherParticipantsDidChangeNotification: NSNotification.Name

A notification that the coordinator posts when its other participants change.

