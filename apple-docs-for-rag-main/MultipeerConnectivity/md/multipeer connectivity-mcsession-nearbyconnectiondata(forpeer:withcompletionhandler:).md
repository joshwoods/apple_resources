

- Multipeer Connectivity
- MCSession
-  nearbyConnectionData(forPeer:withCompletionHandler:) 

Instance Method

# nearbyConnectionData(forPeer:withCompletionHandler:)

Obtains connection data for the specified peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func nearbyConnectionData(
    forPeer peerID: MCPeerID,
    withCompletionHandler completionHandler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func nearbyConnectionData(forPeer peerID: MCPeerID) async throws -> Data
```

## Parameters 

`peerID`  

A peer ID object obtained from the nearby peer that you want to add to a session.

`completionHandler`  

A handler that is called when connection data is available or when an error occurs.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method provides connection data that is required when adding a specific nearby peer to a session if you are using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object. For more information, see the Managing Peers Manually section in the overview of the `MCSession` class reference.

## See Also

### Managing Peers Manually

func connectPeer(MCPeerID, withNearbyConnectionData: Data)

Call this method to connect a peer to the session when using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object.

func cancelConnectPeer(MCPeerID)

Cancels an attempt to connect to a peer.

var connectedPeers: [MCPeerID]

An array of all peers that are currently connected to this session.

