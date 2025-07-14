

- Core Motion
- CMAltimeter
-  isAbsoluteAltitudeAvailable() 

Type Method

# isAbsoluteAltitudeAvailable()

Returns a Boolean value indicating whether the current device reports changes in the absolute altitude.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
class func isAbsoluteAltitudeAvailable() -> Bool
```

## Discussion

Use this method to determine if altitude updates are available before calling the startAbsoluteAltitudeUpdates(to:withHandler:) method.

Note

Absolute altitude is only available on iPhone 12 and later and Apple Watch 6 or SE and later.

## See Also

### Determining Altitude Availability

class func isRelativeAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve altimeter data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

