

- Nearby Interaction
- NISessionDelegate
-  session(\_:didUpdate:) 

Instance Method

# session(\_:didUpdate:)

Notifies you when the session updates nearby objects.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
optional func session(
    _ session: NISession,
    didUpdate nearbyObjects: [NINearbyObject]
)
```

## Parameters 

`session`  

The session that updated.

`nearbyObjects`  

The array of nearby objects that the session updated.

## Mentioned in 

Initiating and maintaining a session

## Discussion

Implement this callback to receive new nearby object updates for the argument session.

In Swift, if a peer is out of range or line of sight, the delegate reads the distance and direction as `nil`. An app can monitor this state and guide a person into range as necessary. For more information, see Initiating and maintaining a session.

In Objective-C, if a peer is out of range or line of sight, the delegate reads the distance as NINearbyObjectDistanceNotAvailable, and direction as NINearbyObjectDirectionNotAvailable.

An app can monitor this state and guide the user into range as necessary. For more information, see Initiating and maintaining a session.

### Provide feedback based on proximity

Apps can react to positional information in an interaction session to create spatial awareness. For example, an app can play audio, invoke haptics, or display visual feedback when a peer is nearby. The following code calls two functions: it calls `enableFunctionalityA` when the device achieves a 1.5-meter proximity to the peer device, and `enableFunctionalityB` when the device achieves a 3-meter proximity to the peer device.

```
func session(_ session: NISession, didUpdate nearbyObjects: [NINearbyObject]) {
    // Ensure there's a current peer token.
    guard let peerToken = peerDiscoveryToken else {
        fatalError("don't have peer token")
    }

    // Find the right peer from session update.
    guard let peerObj = nearbyObjects.first (where: { $0.discoveryToken == peerToken }) else {
        return
    }

    // Retrieve the peer's distance, in meters.
    if let distance = peerObj.distance {
        // Compute peer object's distance.
    }

    // Retrieve the peer's horizontal angle, in radians.
    if let horizontalAngle = peerObj.horizontalAngle {
        // Compute peer object's angle.
    }

    // Retrieve the peer's direction, in `simd_float3`.
    if let direction = peerObj.direction {
        // Compute peer object's direction.
    }
}
```

## See Also

### Monitoring peers

func session(NISession, didGenerateShareableConfigurationData: Data, for: NINearbyObject)

Provides configuration data to share with a third-party accessory.

func session(NISession, didRemove: [NINearbyObject], reason: NINearbyObject.RemovalReason)

Notifies you when the session removes one or more nearby objects.

enum RemovalReason

The reason a session removed a nearby object.

