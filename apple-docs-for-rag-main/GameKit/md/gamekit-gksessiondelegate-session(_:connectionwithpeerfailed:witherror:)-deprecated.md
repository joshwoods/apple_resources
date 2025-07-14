

- GameKit
- GKSessionDelegate
-  session(\_:connectionWithPeerFailed:withError:) Deprecated

Instance Method

# session(\_:connectionWithPeerFailed:withError:)

Received by the delegate when an attempt to connect to another peer failed.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func session(
    _ session: GKSession,
    connectionWithPeerFailed peerID: String,
    withError error: any Error
)
```

## Parameters 

`session`  

The session that received the message.

`peerID`  

A string that uniquely identifies the peer.

`error`  

The error that occurred.

## Discussion

The `error` parameter can be used to inform the user of why the connection failed.

Important

If a GKPeerPickerController object is being used to configure the session, the controller handles this message automatically. Your delegate can ignore it if the peer picker dialog is in use.

## See Also

### Connection Errors

func session(GKSession, didFailWithError: any Error)

Sent to the delegate when a serious error has occurred in the session.

Deprecated

