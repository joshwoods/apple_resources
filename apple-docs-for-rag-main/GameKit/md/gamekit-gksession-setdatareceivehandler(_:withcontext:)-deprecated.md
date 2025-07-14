

- GameKit
- GKSession
-  setDataReceiveHandler(\_:withContext:) Deprecated

Instance Method

# setDataReceiveHandler(\_:withContext:)

Sets the object that handles data received from other peers connected to the session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func setDataReceiveHandler(
    _ handler: Any!,
    withContext context: UnsafeMutableRawPointer!
)
```

## Parameters 

`handler`  

The object you want the session to call when it receives data from other peers.

`context`  

Arbitrary data to be passed to each invocation of the handler.

## Discussion

The handler must implement a method with the following signature:

```
- (void) receiveData:(NSData *)data fromPeer:(NSString *)peer inSession: (GKSession *)session context:(void *)context;
```

where *data* contains the bytes received from a remote peer, *peer* is a string that identifies the peer, *session* is the session that received the data, and *context* is the same context that was passed into the original call to setDataReceiveHandler(_:withContext:).

Important

Data received from other peers should be treated as *untrusted* data. Be sure to validate the data you receive from the session and write your code carefully to avoid security vulnerabilities. See the Secure Coding Guide for more information.

## See Also

### Working with Connected Peers

func send(Data!, toPeers: [Any]!, with: GKSendDataMode) throws

Transmits a collection of bytes to a list of connected peers.

Deprecated

func sendData(toAllPeers: Data!, with: GKSendDataMode) throws

Transmits a collection of bytes to all connected peers.

Deprecated

var disconnectTimeout: TimeInterval

A time interval that expresses how long the session waits before it disconnects a nonresponsive peer.

Deprecated

func disconnectFromAllPeers()

Disconnects the session from all connected peers.

Deprecated

func disconnectPeer(fromAllPeers: String!)

Disconnects a connected peer from all peers connected to the session.

Deprecated

