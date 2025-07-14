

- Multipeer Connectivity
- MCPeerID
-  init(displayName:) 

Initializer

# init(displayName:)

Initializes a peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
init(displayName myDisplayName: String)
```

## Parameters 

`myDisplayName`  

The display name for the local peer. If you use the multipeer browser view controller, this name is shown.

The display name is intended for use in UI elements, and should be short and descriptive of the local peer. The maximum allowable length is 63 bytes in UTF-8 encoding. The `displayName` parameter may not be `nil` or an empty string.

## Return Value

An initialized peer ID object.

## Discussion

Call this method *only* when creating the local peer, not when you create objects that represent other devices.

This method throws an exception if the `displayName` value is too long, empty, or `nil`.

Each call to this method produces a unique peer ID, even for the same display name. If you need a device to maintain a consistent peer ID over time, you may want to archive and reuse it later instead of creating a new one every time your app starts advertising or browsing.

## See Also

### Peer Methods

var displayName: String

The display name for this peer.

