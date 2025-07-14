

- Nearby Interaction
- NINearbyPeerConfiguration
-  peerDiscoveryToken 

Instance Property

# peerDiscoveryToken

A value that uniquely identifies the other peer in the interaction session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
@NSCopying
var peerDiscoveryToken: NIDiscoveryToken { get }
```

## Discussion

NI sets this property to the value of the peer discovery token you pass to the init(peerToken:) initializer.

