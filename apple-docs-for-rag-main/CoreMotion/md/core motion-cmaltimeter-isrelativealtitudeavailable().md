

- Core Motion
- CMAltimeter
-  isRelativeAltitudeAvailable() 

Type Method

# isRelativeAltitudeAvailable()

Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class func isRelativeAltitudeAvailable() -> Bool
```

## Return Value

true if the device supports relative altitude changes or false if it does not.

## Discussion

Use this method to determine if altitude updates are available before calling the startRelativeAltitudeUpdates(to:withHandler:) method.

## See Also

### Determining Altitude Availability

class func isAbsoluteAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device reports changes in the absolute altitude.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve altimeter data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

