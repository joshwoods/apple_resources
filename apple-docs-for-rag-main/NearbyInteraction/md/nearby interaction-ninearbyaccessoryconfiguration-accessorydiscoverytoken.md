

- Nearby Interaction
- NINearbyAccessoryConfiguration
-  accessoryDiscoveryToken 

Instance Property

# accessoryDiscoveryToken

An identifier for the accessory in a session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
@NSCopying
var accessoryDiscoveryToken: NIDiscoveryToken { get }
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

The value of this property refers to a specific peer accessory. To match distance updates your app receives through a session with a peer using session(_:didUpdate:), compare the argument object’s discovery token with the value of this property.

Subsequent sessions with the same peer device produce a different value for this property. For user privacy, the system assigns a random number unique to the session that prevents the correlation of this property with a particular device.

