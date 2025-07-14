

- Core Motion
- CMAltimeter
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns a value indicating whether the app is authorized to retrieve altimeter data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+watchOS 4.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

## See Also

### Determining Altitude Availability

class func isAbsoluteAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device reports changes in the absolute altitude.

class func isRelativeAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes.

enum CMAuthorizationStatus

The authorization status for motion-related features.

