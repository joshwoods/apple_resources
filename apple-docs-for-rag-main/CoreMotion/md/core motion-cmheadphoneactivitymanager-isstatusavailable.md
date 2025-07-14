

- Core Motion
- CMHeadphoneActivityManager
-  isStatusAvailable 

Instance Property

# isStatusAvailable

A Boolean value that indicates whether the current device supports headphone status.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
var isStatusAvailable: Bool { get }
```

## See Also

### Checking Availability

var isActivityAvailable: Bool

A Boolean value that indicates whether the current device supports headphone activity.

var isActivityActive: Bool

A Boolean value that indicates whether headphone motion activity is active.

var isStatusActive: Bool

A Boolean value that indicates whether headphone status is active.

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone activity.

