

- AVFoundation
- AVPlaybackCoordinator
-  otherParticipants 

Instance Property

# otherParticipants

The identifiers of the other participants in a group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var otherParticipants: [AVCoordinatedPlaybackParticipant] { get }
```

## Discussion

Use this property value to create a user interface that informs the user about the state of other participants in the group.

Note

To observe changes to this property value, register for notifications of type otherParticipantsDidChangeNotification.

## See Also

### Observing Other Participants

class AVCoordinatedPlaybackParticipant

An object that represents a participant in a coordinated playback session.

class let otherParticipantsDidChangeNotification: NSNotification.Name

A notification that the coordinator posts when its other participants change.

