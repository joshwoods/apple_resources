

- Nearby Interaction
- NINearbyPeerConfiguration
-  init(peerToken:) 

Initializer

# init(peerToken:)

Creates a configuration for interaction between devices, including iPhone and Apple Watch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
init(peerToken: NIDiscoveryToken)
```

## Parameters 

`peerToken`  

The value of another device’s discovery token. This value uniquely identifies the other peer in the interaction session.

## Mentioned in 

Initiating and maintaining a session

## Discussion

To acquire a peer’s discovery token, two instantiations of the app exchange their respective discoveryToken over the network using a method you choose. For a discussion that covers sharing discovery tokens using Multipeer Connectivity, see Discovering peers with Multipeer Connectivity.

