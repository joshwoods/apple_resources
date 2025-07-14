

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:didReceiveInvitationFromParticipantID:callID:) Deprecated

Instance Method

# voiceChatService(\_:didReceiveInvitationFromParticipantID:callID:)

Asks the client to accept or reject an invitation from a remote participant.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    didReceiveInvitationFromParticipantID participantID: String,
    callID: Int
)
```

## Parameters 

`voiceChatService`  

The service that received the request.

`participantID`  

A string that uniquely identifies the other user.

`callID`  

An integer that uniquely identifies the request.

## Discussion

If this method is not implemented by the client, the voice chat service automatically accept requests from other participants.

This method should call the service’s acceptCallID(_:) method if it wants to accept the request or the denyCallID(_:) to reject it.

