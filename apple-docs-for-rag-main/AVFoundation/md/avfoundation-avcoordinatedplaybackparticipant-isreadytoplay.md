

- AVFoundation
- AVCoordinatedPlaybackParticipant
-  isReadyToPlay 

Instance Property

# isReadyToPlay

A Boolean value that indicates whether the participant is ready to start coordinated playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var isReadyToPlay: Bool { get }
```

## See Also

### Accessing Participant Status

var identifier: UUID

A unique identifier for the participant.

var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason]

The reasons a participant isn’t currently participating in coordinated playback.

