

- Core Motion
- CMPedometer
-  isStepCountingAvailable() 

Type Method

# isStepCountingAvailable()

Returns a Boolean value indicating whether step counting is available on the current device.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
class func isStepCountingAvailable() -> Bool
```

## Return Value

true if step counting is available or false if it is not.

## See Also

### Determining Pedometer Availability

class func isDistanceAvailable() -> Bool

Returns a Boolean value indicating whether distance estimation is available on the current device.

class func isFloorCountingAvailable() -> Bool

Returns a Boolean value indicating whether floor counting is available on the current device.

class func isPaceAvailable() -> Bool

Returns a Boolean value indicating whether pace information is available on the current device.

class func isCadenceAvailable() -> Bool

Returns a Boolean value indicating whether cadence information is available on the current device.

class func isPedometerEventTrackingAvailable() -> Bool

Returns a Boolean value indicating whether pedometer events are available on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to gather pedometer data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

