

- Watch Connectivity
- WCSession
-  iOSDeviceNeedsUnlockAfterRebootForReachability 

Instance Property

# iOSDeviceNeedsUnlockAfterRebootForReachability

A Boolean value indicating whether the paired iPhone must be in an unlocked state to be reachable.

watchOS 2.0+

``` source
var iOSDeviceNeedsUnlockAfterRebootForReachability: Bool { get }
```

## Discussion

When the isReachable property is false, use this property to determine if the iPhone is unreachable because it needs to be unlocked first. A recently rebooted iPhone remains unreachable until the user unlocks it for the first time. Until the user unlocks the iPhone, the value of this property is true. When the value is true, you might display an alert from your Watch app asking the user to unlock the iPhone to continue. After the user unlocks the iPhone, the value of the property changes to false.

The value in this property is valid only for a configured session that has been activated successfully. If the activationState property is available, its value must be WCSessionActivationState.activated. When the session becomes inactive or deactivated, you should ignore the value in this property.

## See Also

### Getting the Paired Device Information

var isPaired: Bool

A Boolean indicating whether the current iPhone has a paired Apple Watch.

var isWatchAppInstalled: Bool

A Boolean value indicating whether the currently paired and active Apple Watch has installed the app.

var isCompanionAppInstalled: Bool

A Boolean value indicating whether the companion has installed the app.

var isComplicationEnabled: Bool

A Boolean value indicating whether the Watch app’s complication is in use on the currently paired and active Apple Watch.

var watchDirectoryURL: URL?

A directory for storing information specific to the currently paired and active Apple Watch.

