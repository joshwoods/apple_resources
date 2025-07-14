

- Watch Connectivity
- WCSession
-  isWatchAppInstalled 

Instance Property

# isWatchAppInstalled

A Boolean value indicating whether the currently paired and active Apple Watch has installed the app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
var isWatchAppInstalled: Bool { get }
```

## Discussion

The user can choose to install only a subset of available apps on Apple Watch. The value of this property is true when the Watch app associated with the current iOS app is installed on the user’s Apple Watch or false when it is not installed.

The value in this property is valid only for a configured session that has been activated successfully. If the activationState property is available, its value must be WCSessionActivationState.activated. When the session becomes inactive or deactivated, you should ignore the value in this property.

## See Also

### Getting the Paired Device Information

var isPaired: Bool

A Boolean indicating whether the current iPhone has a paired Apple Watch.

var iOSDeviceNeedsUnlockAfterRebootForReachability: Bool

A Boolean value indicating whether the paired iPhone must be in an unlocked state to be reachable.

var isCompanionAppInstalled: Bool

A Boolean value indicating whether the companion has installed the app.

var isComplicationEnabled: Bool

A Boolean value indicating whether the Watch app’s complication is in use on the currently paired and active Apple Watch.

var watchDirectoryURL: URL?

A directory for storing information specific to the currently paired and active Apple Watch.

