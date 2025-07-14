

- Core Motion
- CMHeadphoneMotionManager
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns the authorization status for monitoring headphone motion.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

## See Also

### Checking Availability

var isDeviceMotionAvailable: Bool

A Boolean value that indicates whether the current device supports the headphone motion manager.

var isDeviceMotionActive: Bool

A Boolean value that indicates whether the headphone motion manager is active.

var isConnectionStatusActive: Bool

