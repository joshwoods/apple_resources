

- GameKit
- GKVoiceChatService
-  receivedRealTime(\_:fromParticipantID:) Deprecated

Instance Method

# receivedRealTime(\_:fromParticipantID:)

Called by the client to deliver voice data received from a remote participant..

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func receivedRealTime(
    _ audio: Data!,
    fromParticipantID participantID: String!
)
```

Deprecated

Use SharePlay instead

## Parameters 

`audio`  

The audio data that was received from the other participant.

`participantID`  

A string that uniquely identifies the speaking participant.

## Discussion

The voice chat service uses a network connection provided by the client to exchange information between the participants. When the client receives information intended for the voice chat service, it should call this method to transfer it.

## See Also

### Related Documentation

func voiceChatService(GKVoiceChatService, sendRealTime: Data, toParticipantID: String)

Asks the client to send data to a participant that must get there quickly.

Deprecated

### Methods Called by the Client

func acceptCallID(Int) throws

Accepts a request from a remote user to establish a voice chat.

Deprecated

func denyCallID(Int)

Rejects a request to establish a voice chat.

Deprecated

func receivedData(Data!, fromParticipantID: String!)

Called by the client to deliver new data received from a remote participant.

Deprecated

