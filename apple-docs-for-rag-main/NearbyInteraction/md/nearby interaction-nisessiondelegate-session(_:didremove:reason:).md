

- Nearby Interaction
- NISessionDelegate
-  session(\_:didRemove:reason:) 

Instance Method

# session(\_:didRemove:reason:)

Notifies you when the session removes one or more nearby objects.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
optional func session(
    _ session: NISession,
    didRemove nearbyObjects: [NINearbyObject],
    reason: NINearbyObject.RemovalReason
)
```

## Parameters 

`session`  

The session that removed a tracked object or objects.

`nearbyObjects`  

The tracked objects the session removed.

`reason`  

The reason the session removed the objects.

## Mentioned in 

Initiating and maintaining a session

## Discussion

The session invokes this callback to notify an app when an interaction ended for the argument `reason`. After Nearby Interaction calls this function, the framework no longer calls session(_:didUpdate:) for the argument `trackedObjects`.

### Restart the Session on Timeout

A peer may exceed the supported range for too long or a session may fail to start after the initial attempt. If the peer remains nearby or comes back within the supported range, an app may want to try again. To handle this situation, check for NINearbyObject.RemovalReason.timeout in this callback and then restart the session. In the following code, the app implements a hypothetical `shouldResume(_:NINearbyObject)` function with app-specific logic that determinations whether to retry. The function may check how many times it’s retried and failed, whether an accessory indicated it stopped, and whether the existing configuration suffices unchanged. Then, the app calls run(_:) again on the session.

```
func session(_ session: NISession, didRemove nearbyObjects: [NINearbyObject],
        reason: NINearbyObject.RemovalReason) {

    // Only retry if the peer timed out.
    guard reason == .timeout else { return }

    // The session runs with one accessory.
    guard let peer = nearbyObjects.first else { return }

    if shouldResume(peer) {
        // Restart the session.
        if let config = session.configuration {
            session.run(config)
        }
    }
}
```

## See Also

### Monitoring peers

func session(NISession, didUpdate: [NINearbyObject])

Notifies you when the session updates nearby objects.

func session(NISession, didGenerateShareableConfigurationData: Data, for: NINearbyObject)

Provides configuration data to share with a third-party accessory.

enum RemovalReason

The reason a session removed a nearby object.

