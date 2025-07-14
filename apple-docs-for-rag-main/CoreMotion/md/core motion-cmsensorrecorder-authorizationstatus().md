

- Core Motion
- CMSensorRecorder
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns a value indicating whether the app is authorized to record sensor data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+watchOS 4.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

## See Also

### Checking the Availability of Sensor Recording

class func isAccelerometerRecordingAvailable() -> Bool

Returns a Boolean value indicating whether accelerometer recording is supported on the current device.

enum CMAuthorizationStatus

The authorization status for motion-related features.

class func isAuthorizedForRecording() -> Bool

Returns a Boolean value indicating whether the app is authorized to record sensor data.

Deprecated

