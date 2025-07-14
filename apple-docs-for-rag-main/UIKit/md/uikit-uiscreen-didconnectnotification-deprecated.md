

- UIKit
- UIScreen
-  didConnectNotification Deprecated

Type Property

# didConnectNotification

A notification the system posts when a new screen connects to the device.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOSDeprecated

``` source
nonisolated
class let didConnectNotification: NSNotification.Name
```

Deprecated

Use the scene(_:willConnectTo:options:) method on a scene delegate or willConnectNotification to recieve notification of connecting scenes from other screens.

## Mentioned in 

Processing queued notifications

## Discussion

Connection notifications aren’t sent for screens that are already present when the app launches. The app can instead use the screens method to get the current set of screens at launch time.

The object of the notification is the UIScreen object representing the new screen. There’s no `userInfo` dictionary.

## See Also

### Deprecated notifications

class let didDisconnectNotification: NSNotification.Name

A notification the system posts when a screen disconnects from the device.

Deprecated

