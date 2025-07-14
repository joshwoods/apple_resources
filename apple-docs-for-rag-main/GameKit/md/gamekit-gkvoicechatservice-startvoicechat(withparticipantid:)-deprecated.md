

- GameKit
- GKVoiceChatService
-  startVoiceChat(withParticipantID:) Deprecated

Instance Method

# startVoiceChat(withParticipantID:)

Sends a request to another participant to join the voice chat.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func startVoiceChat(withParticipantID participantID: String!) throws
```

Deprecated

Use SharePlay instead

## Parameters 

`participantID`  

A string that uniquely identifies the participant to connect to.

## Discussion

The voice chat service calls the client’s voiceChatService(_:send:toParticipantID:) method to send the connection request to the remote participant.

