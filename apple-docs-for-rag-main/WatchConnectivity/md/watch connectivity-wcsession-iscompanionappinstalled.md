

- Watch Connectivity
- WCSession
-  isCompanionAppInstalled 

Instance Property

# isCompanionAppInstalled

A Boolean value indicating whether the companion has installed the app.

watchOS 6.0+

``` source
var isCompanionAppInstalled: Bool { get }
```

## Discussion

Use this property on independent watchOS apps to determine whether the paired iPhone has installed the app.

## See Also

### Getting the Paired Device Information

var isPaired: Bool

A Boolean indicating whether the current iPhone has a paired Apple Watch.

var iOSDeviceNeedsUnlockAfterRebootForReachability: Bool

A Boolean value indicating whether the paired iPhone must be in an unlocked state to be reachable.

var isWatchAppInstalled: Bool

A Boolean value indicating whether the currently paired and active Apple Watch has installed the app.

var isComplicationEnabled: Bool

A Boolean value indicating whether the Watch app’s complication is in use on the currently paired and active Apple Watch.

var watchDirectoryURL: URL?

A directory for storing information specific to the currently paired and active Apple Watch.

