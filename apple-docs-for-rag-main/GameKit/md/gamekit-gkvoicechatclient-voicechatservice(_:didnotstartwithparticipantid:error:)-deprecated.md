

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:didNotStartWithParticipantID:error:) Deprecated

Instance Method

# voiceChatService(\_:didNotStartWithParticipantID:error:)

Received by the client when an attempt to establish a voice chat with another participant failed.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    didNotStartWithParticipantID participantID: String,
    error: (any Error)?
)
```

## Parameters 

`voiceChatService`  

The voice chat service that was establishing the connection.

`participantID`  

A string that uniquely identifies the other user.

`error`  

The error that prevented the voice chat from being established.

## Discussion

Your application can implement this method to notify the user that an error occurred when establishing a connection.

## See Also

### Responding to Changes in Other Participants

func voiceChatService(GKVoiceChatService, didStartWithParticipantID: String)

Received by the client when a voice chat with another participant is established.

Deprecated

func voiceChatService(GKVoiceChatService, didStopWithParticipantID: String, error: (any Error)?)

Received by the client when a previously established voice chat has ended.

Deprecated

