

- Core Motion
- CMHeadphoneActivityManager
-  isStatusActive 

Instance Property

# isStatusActive

A Boolean value that indicates whether headphone status is active.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
var isStatusActive: Bool { get }
```

## See Also

### Checking Availability

var isActivityAvailable: Bool

A Boolean value that indicates whether the current device supports headphone activity.

var isActivityActive: Bool

A Boolean value that indicates whether headphone motion activity is active.

var isStatusAvailable: Bool

A Boolean value that indicates whether the current device supports headphone status.

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone activity.

