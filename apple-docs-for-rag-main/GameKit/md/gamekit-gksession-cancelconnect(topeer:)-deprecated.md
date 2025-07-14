

- GameKit
- GKSession
-  cancelConnect(toPeer:) Deprecated

Instance Method

# cancelConnect(toPeer:)

Cancels a pending request to connect to another iOS device.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func cancelConnect(toPeer peerID: String!)
```

## Parameters 

`peerID`  

The string identifying the peer you previously requested to connect to.

## Discussion

Your application previously called connect(toPeer:withTimeout:) to create a connection to another iOS device. When your application cancels the connection attempt, both delegates’ session(_:connectionWithPeerFailed:withError:) methods are called.

If your application already connected to the peer, your application should call disconnectFromAllPeers() instead.

## See Also

### Connecting to a Remote Peer

func connect(toPeer: String!, withTimeout: TimeInterval)

Creates a connection to another iOS device.

Deprecated

