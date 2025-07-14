

- AVFoundation
- AVPlaybackCoordinator
-  otherParticipantsDidChangeNotification 

Type Property

# otherParticipantsDidChangeNotification

A notification that the coordinator posts when its other participants change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class let otherParticipantsDidChangeNotification: NSNotification.Name
```

## See Also

### Observing Other Participants

var otherParticipants: [AVCoordinatedPlaybackParticipant]

The identifiers of the other participants in a group.

class AVCoordinatedPlaybackParticipant

An object that represents a participant in a coordinated playback session.

