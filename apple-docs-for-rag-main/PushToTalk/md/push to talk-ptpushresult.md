

- Push to Talk
-  PTPushResult 

Class

# PTPushResult

An object that represents a push result.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class PTPushResult
```

## Mentioned in 

Creating a Push to Talk app

## Overview

When an app receives an Apple Push Notification service payload, return a PTPushResult object as part of the delegate method. Use activeRemoteParticipant(_:) to show the latest participant information in the system user interface. Create a push result with leaveChannel to remove a user from the channel.

```
func incomingPushResult(channelManager: PTChannelManager,
                        channelUUID: UUID,
                        pushPayload: [String: Any]) -> PTPushResult {
    guard let activeSpeaker = pushPayload["activeSpeaker"] as? String else {
        // Report that there's no active speaker, so leave the channel.
        return .leaveChannel
    }

    let activeSpeakerImage = // Get the cached image for the active speaker.
    let participant = PTParticipant(name: activeSpeaker,
                                    image: activeSpeakerImage)
    // Report the active participant information to the system.
    return .activeRemoteParticipant(participant)
}
```

## Topics

### Updating the active participant

class func activeRemoteParticipant(PTParticipant) -> PTPushResult

Creates a push result for reporting that a remote participant started to speak.

### Leaving the channel

class var leaveChannel: PTPushResult

Creates a push result for leaving a channel.

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

