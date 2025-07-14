

- Core Motion
- CMPedometer
-  isPedometerEventTrackingAvailable() 

Type Method

# isPedometerEventTrackingAvailable()

Returns a Boolean value indicating whether pedometer events are available on the current device.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+watchOS 3.0+

``` source
class func isPedometerEventTrackingAvailable() -> Bool
```

## Return Value

true if pedometer events are available or false if they are not.

## See Also

### Determining Pedometer Availability

class func isStepCountingAvailable() -> Bool

Returns a Boolean value indicating whether step counting is available on the current device.

class func isDistanceAvailable() -> Bool

Returns a Boolean value indicating whether distance estimation is available on the current device.

class func isFloorCountingAvailable() -> Bool

Returns a Boolean value indicating whether floor counting is available on the current device.

class func isPaceAvailable() -> Bool

Returns a Boolean value indicating whether pace information is available on the current device.

class func isCadenceAvailable() -> Bool

Returns a Boolean value indicating whether cadence information is available on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to gather pedometer data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

