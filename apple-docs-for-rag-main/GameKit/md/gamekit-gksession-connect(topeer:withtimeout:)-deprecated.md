

- GameKit
- GKSession
-  connect(toPeer:withTimeout:) Deprecated

Instance Method

# connect(toPeer:withTimeout:)

Creates a connection to another iOS device.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func connect(
    toPeer peerID: String!,
    withTimeout timeout: TimeInterval
)
```

## Parameters 

`peerID`  

The string that identifies the peer to connect to.

`timeout`  

The amount of time to wait before canceling the connection attempt.

## Discussion

When your application is acting as a client, it calls this method to connect to an available peer it discovered. When your application calls this method, a request is transmitted to the remote peer, who chooses whether to accept or reject the connection request.

If the connection to the remote peer is successful, the delegate’s session(_:peer:didChange:) method is called for each peer it successfully connected to. If the connection fails or your application cancels the connection attempt, the session calls the delegate’s session(_:connectionWithPeerFailed:withError:) method.

## See Also

### Connecting to a Remote Peer

func cancelConnect(toPeer: String!)

Cancels a pending request to connect to another iOS device.

Deprecated

