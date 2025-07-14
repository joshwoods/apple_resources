

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:didStartWithParticipantID:) Deprecated

Instance Method

# voiceChatService(\_:didStartWithParticipantID:)

Received by the client when a voice chat with another participant is established.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    didStartWithParticipantID participantID: String
)
```

## Parameters 

`voiceChatService`  

The voice chat service that initiated the connection.

`participantID`  

A string that uniquely identifies the other user.

## Discussion

Your client can use this method to update the user interface to show that a connection has been established.

## See Also

### Responding to Changes in Other Participants

func voiceChatService(GKVoiceChatService, didNotStartWithParticipantID: String, error: (any Error)?)

Received by the client when an attempt to establish a voice chat with another participant failed.

Deprecated

func voiceChatService(GKVoiceChatService, didStopWithParticipantID: String, error: (any Error)?)

Received by the client when a previously established voice chat has ended.

Deprecated

