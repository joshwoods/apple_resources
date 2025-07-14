

- GameKit
- GKVoiceChatService
-  acceptCallID(\_:) Deprecated

Instance Method

# acceptCallID(\_:)

Accepts a request from a remote user to establish a voice chat.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func acceptCallID(_ callID: Int) throws
```

Deprecated

Use SharePlay instead

## Parameters 

`callID`  

An integer that identifies the connection request.

## Discussion

When a remote user requests a voice chat, the voice chat service calls the client’s voiceChatService(_:didReceiveInvitationFromParticipantID:callID:) method. The client calls this method to accept the request or denyCallID(_:) to reject it.

## See Also

### Methods Called by the Client

func denyCallID(Int)

Rejects a request to establish a voice chat.

Deprecated

func receivedData(Data!, fromParticipantID: String!)

Called by the client to deliver new data received from a remote participant.

Deprecated

func receivedRealTime(Data!, fromParticipantID: String!)

Called by the client to deliver voice data received from a remote participant..

Deprecated

