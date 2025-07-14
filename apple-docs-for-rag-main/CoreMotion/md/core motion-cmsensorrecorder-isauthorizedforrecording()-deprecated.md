

- Core Motion
- CMSensorRecorder
-  isAuthorizedForRecording() Deprecated

Type Method

# isAuthorizedForRecording()

Returns a Boolean value indicating whether the app is authorized to record sensor data.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–4.0Deprecated

``` source
class func isAuthorizedForRecording() -> Bool
```

Deprecated

Use authorizationStatus() instead.

## Return Value

true if the app is authorized to record sensor data or false if it is not.

## See Also

### Checking the Availability of Sensor Recording

class func isAccelerometerRecordingAvailable() -> Bool

Returns a Boolean value indicating whether accelerometer recording is supported on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to record sensor data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

