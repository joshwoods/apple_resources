

- GameKit
- GKSession
-  sendData(toAllPeers:with:) Deprecated

Instance Method

# sendData(toAllPeers:with:)

Transmits a collection of bytes to all connected peers.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
func sendData(
    toAllPeers data: Data!,
    with mode: GKSendDataMode
) throws
```

Deprecated

No longer supported.

## Parameters 

`data`  

The bytes to be sent.

`mode`  

The mechanism used to send the data.

## Discussion

The session queues the data and transmits it when the network is free.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Working with Connected Peers

func setDataReceiveHandler(Any!, withContext: UnsafeMutableRawPointer!)

Sets the object that handles data received from other peers connected to the session.

Deprecated

func send(Data!, toPeers: [Any]!, with: GKSendDataMode) throws

Transmits a collection of bytes to a list of connected peers.

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

