

- GameKit
- GKVoiceChatClient
-  voiceChatService(\_:sendRealTime:toParticipantID:) Deprecated

Instance Method

# voiceChatService(\_:sendRealTime:toParticipantID:)

Asks the client to send data to a participant that must get there quickly.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func voiceChatService(
    _ voiceChatService: GKVoiceChatService,
    sendRealTime data: Data,
    toParticipantID participantID: String
)
```

## Parameters 

`voiceChatService`  

The service that requested the transmission.

`data`  

The data to send.

`participantID`  

A string that uniquely identifies the participant to send the data to.

## Discussion

An implementation of this method maps the `participantID` string to a known participant and transmits the data to them. Data transmitted by this method can be sent unreliably. When the client on the other end receives this data, it should forward it to the voice chat service by calling the service’s receivedRealTime(_:fromParticipantID:) method.

## See Also

### Sending data to other participants

func voiceChatService(GKVoiceChatService, send: Data, toParticipantID: String)

A request for the client to send data to a participant.

**Required**

Deprecated

