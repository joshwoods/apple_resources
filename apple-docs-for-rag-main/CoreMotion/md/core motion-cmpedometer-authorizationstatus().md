

- Core Motion
- CMPedometer
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns a value indicating whether the app is authorized to gather pedometer data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+watchOS 4.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

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

class func isPedometerEventTrackingAvailable() -> Bool

Returns a Boolean value indicating whether pedometer events are available on the current device.

enum CMAuthorizationStatus

The authorization status for motion-related features.

