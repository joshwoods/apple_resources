

- GameKit
- GKSession
-  disconnectFromAllPeers() Deprecated

Instance Method

# disconnectFromAllPeers()

Disconnects the session from all connected peers.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func disconnectFromAllPeers()
```

## See Also

### Working with Connected Peers

func setDataReceiveHandler(Any!, withContext: UnsafeMutableRawPointer!)

Sets the object that handles data received from other peers connected to the session.

Deprecated

func send(Data!, toPeers: [Any]!, with: GKSendDataMode) throws

Transmits a collection of bytes to a list of connected peers.

Deprecated

func sendData(toAllPeers: Data!, with: GKSendDataMode) throws

Transmits a collection of bytes to all connected peers.

Deprecated

var disconnectTimeout: TimeInterval

A time interval that expresses how long the session waits before it disconnects a nonresponsive peer.

Deprecated

func disconnectPeer(fromAllPeers: String!)

Disconnects a connected peer from all peers connected to the session.

Deprecated

