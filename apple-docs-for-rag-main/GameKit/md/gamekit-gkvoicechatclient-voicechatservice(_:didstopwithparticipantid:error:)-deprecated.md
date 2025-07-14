

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:didStopWithParticipantID:error:) Deprecated

Instance Method

# voiceChatService(\_:didStopWithParticipantID:error:)

Received by the client when a previously established voice chat has ended.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    didStopWithParticipantID participantID: String,
    error: (any Error)?
)
```

## Parameters 

`voiceChatService`  

The voice chat that maintained the connection.

`participantID`  

A string that uniquely identifies the user who disconnected.

`error`  

The error that caused the chat to end.

## Discussion

Your application can implement this method to notify the user that an established voice connection has ended. This may occur when another participant ends the chat or if the network connection was lost.

## See Also

### Responding to Changes in Other Participants

func voiceChatService(GKVoiceChatService, didStartWithParticipantID: String)

Received by the client when a voice chat with another participant is established.

Deprecated

func voiceChatService(GKVoiceChatService, didNotStartWithParticipantID: String, error: (any Error)?)

Received by the client when an attempt to establish a voice chat with another participant failed.

Deprecated

