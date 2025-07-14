

- Core Motion
- CMPedometer
-  isPaceAvailable() 

Type Method

# isPaceAvailable()

Returns a Boolean value indicating whether pace information is available on the current device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
class func isPaceAvailable() -> Bool
```

## Return Value

true if pace information is available or false if it is not.

## Discussion

Pace measurement indicates the ability to determine the user’s pace in seconds per meter. This capability is not supported on all devices.

## See Also

### Determining Pedometer Availability

class func isStepCountingAvailable() -> Bool

Returns a Boolean value indicating whether step counting is available on the current device.

class func isDistanceAvailable() -> Bool

Returns a Boolean value indicating whether distance estimation is available on the current device.

class func isFloorCountingAvailable() -> Bool

Returns a Boolean value indicating whether floor counting is available on the current device.

class func isCadenceAvailable() -> Bool

Returns a Boolean value indicating whether cadence information is available on the current device.

class func isPedometerEventTrackingAvailable() -> Bool

Returns a Boolean value indicating whether pedometer events are available on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to gather pedometer data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

