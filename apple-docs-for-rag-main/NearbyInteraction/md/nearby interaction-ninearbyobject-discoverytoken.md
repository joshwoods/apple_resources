

- Nearby Interaction
- NINearbyObject
-  discoveryToken 

Instance Property

# discoveryToken

A unique identifier for a peer device in the session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
@NSCopying
var discoveryToken: NIDiscoveryToken { get }
```

## Mentioned in 

Discovering peers with Multipeer Connectivity

## Discussion

The value of this property refers to a specific peer device. Your session delegate receives updates for a peer’s position in your delegate’s session(_:didUpdate:) implementation. To correspond the updates to an iPhone or Apple Watch among multiple peer devices with which your app interacts, compare the value of this property to the configuration’s peerDiscoveryToken. For interactions with third-party accessories, compare the value of this property to the configuration’s accessoryDiscoveryToken.

Subsequent sessions with the same peer device produce a different value for this property. For user privacy, the system assigns this property a unique, random number to prevent correlation between this property and a particular device.

