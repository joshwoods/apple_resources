

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:send:toParticipantID:) Deprecated

Instance Method

# voiceChatService(\_:send:toParticipantID:)

A request for the client to send data to a participant.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    send data: Data,
    toParticipantID participantID: String
)
```

**Required**

## Parameters 

`voiceChatService`  

The service that requested the transmission.

`data`  

The data to send.

`participantID`  

A string that uniquely identifies the participant to send the data to.

## Discussion

An implementation of this method must reliably transmit the data to the participant identified by `participantID`. When the client on the other end receives the data, it should forward it to the voice chat service by calling the service’s receivedData(_:fromParticipantID:) method.

## See Also

### Sending data to other participants

func voiceChatService(GKVoiceChatService, sendRealTime: Data, toParticipantID: String)

Asks the client to send data to a participant that must get there quickly.

Deprecated

