

- Core Motion
- CMHeadphoneActivityManager
-  isActivityActive 

Instance Property

# isActivityActive

A Boolean value that indicates whether headphone motion activity is active.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
var isActivityActive: Bool { get }
```

## See Also

### Checking Availability

var isActivityAvailable: Bool

A Boolean value that indicates whether the current device supports headphone activity.

var isStatusAvailable: Bool

A Boolean value that indicates whether the current device supports headphone status.

var isStatusActive: Bool

A Boolean value that indicates whether headphone status is active.

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone activity.

