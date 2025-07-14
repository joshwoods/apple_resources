

- GameKit
- GKSession
-  send(\_:toPeers:with:) Deprecated

Instance Method

# send(\_:toPeers:with:)

Transmits a collection of bytes to a list of connected peers.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
func send(
    _ data: Data!,
    toPeers peers: [Any]!,
    with mode: GKSendDataMode
) throws
```

Deprecated

No longer supported.

## Parameters 

`data`  

The bytes to be sent.

`peers`  

An array of NSString objects identifying the peers that should receive the data.

`mode`  

The mechanism used to send the data.

## Discussion

The session queues the data and transmits it in the order it was queued. Data transmitted unreliably may be received out of order by the other peers.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Working with Connected Peers

func setDataReceiveHandler(Any!, withContext: UnsafeMutableRawPointer!)

Sets the object that handles data received from other peers connected to the session.

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

