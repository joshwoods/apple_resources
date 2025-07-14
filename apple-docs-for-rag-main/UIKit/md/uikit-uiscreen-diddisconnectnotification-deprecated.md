

- UIKit
- UIScreen
-  didDisconnectNotification Deprecated

Type Property

# didDisconnectNotification

A notification the system posts when a screen disconnects from the device.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOSDeprecated

``` source
nonisolated
class let didDisconnectNotification: NSNotification.Name
```

Deprecated

Use the sceneDidDisconnect(_:) method on a scene delegate or didDisconnectNotification to recieve notification of disconnecting scenes from other screens.

## Mentioned in 

Processing queued notifications

## Discussion

The object of the notification is the UIScreen object that represented the now-disconnected screen. There’s no `userInfo` dictionary.

## See Also

### Deprecated notifications

class let didConnectNotification: NSNotification.Name

A notification the system posts when a new screen connects to the device.

Deprecated

