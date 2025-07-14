

- Core Motion
- CMHeadphoneMotionManager
-  isDeviceMotionAvailable 

Instance Property

# isDeviceMotionAvailable

A Boolean value that indicates whether the current device supports the headphone motion manager.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
var isDeviceMotionAvailable: Bool { get }
```

## See Also

### Checking Availability

var isDeviceMotionActive: Bool

A Boolean value that indicates whether the headphone motion manager is active.

var isConnectionStatusActive: Bool

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone motion.

