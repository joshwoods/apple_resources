

- Core Motion
- CMMotionActivityManager
-  isActivityAvailable() 

Type Method

# isActivityAvailable()

Returns a Boolean indicating whether motion data is available on the current device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class func isActivityAvailable() -> Bool
```

## Return Value

true if motion data is available or false if it is not.

## Discussion

Motion data is not available on all iOS devices. Use this method to determine if support is available on the current device.

## See Also

### Determining Activity Availability

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve stored motion data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

