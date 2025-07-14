

- GameKit
- GKVoiceChatService
-  stopVoiceChat(withParticipantID:) Deprecated

Instance Method

# stopVoiceChat(withParticipantID:)

Ends a previously established voice chat.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func stopVoiceChat(withParticipantID participantID: String!)
```

Deprecated

Use SharePlay instead

## Parameters 

`participantID`  

A string that uniquely identifies the participant in the chat.

## Discussion

When this method is called, the client’s voiceChatService(_:didStopWithParticipantID:error:) method is called.

