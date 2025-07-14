

- Core Motion
- CMMotionActivityManager
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns a value indicating whether the app is authorized to retrieve stored motion data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+watchOS 4.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

## See Also

### Determining Activity Availability

class func isActivityAvailable() -> Bool

Returns a Boolean indicating whether motion data is available on the current device.

enum CMAuthorizationStatus

The authorization status for motion-related features.

