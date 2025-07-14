

- AVFoundation
- AVCoordinatedPlaybackParticipant
-  identifier 

Instance Property

# identifier

A unique identifier for the participant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var identifier: UUID { get }
```

## See Also

### Accessing Participant Status

var isReadyToPlay: Bool

A Boolean value that indicates whether the participant is ready to start coordinated playback.

var suspensionReasons: [AVCoordinatedPlaybackSuspension.Reason]

The reasons a participant isn’t currently participating in coordinated playback.

