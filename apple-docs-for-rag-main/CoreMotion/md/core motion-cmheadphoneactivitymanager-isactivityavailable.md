

- Core Motion
- CMHeadphoneActivityManager
-  isActivityAvailable 

Instance Property

# isActivityAvailable

A Boolean value that indicates whether the current device supports headphone activity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
var isActivityAvailable: Bool { get }
```

## Discussion

If the device supports headphone activity, start status updates and then wait for an update that indicates supported headphones are connected.

## See Also

### Checking Availability

var isActivityActive: Bool

A Boolean value that indicates whether headphone motion activity is active.

var isStatusAvailable: Bool

A Boolean value that indicates whether the current device supports headphone status.

var isStatusActive: Bool

A Boolean value that indicates whether headphone status is active.

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone activity.

