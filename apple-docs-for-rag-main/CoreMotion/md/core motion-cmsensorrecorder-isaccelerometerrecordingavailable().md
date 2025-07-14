

- Core Motion
- CMSensorRecorder
-  isAccelerometerRecordingAvailable() 

Type Method

# isAccelerometerRecordingAvailable()

Returns a Boolean value indicating whether accelerometer recording is supported on the current device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class func isAccelerometerRecordingAvailable() -> Bool
```

## Return Value

true if accelerometer recording is available or false if it is not.

## Discussion

Call this method before trying to record or retrieve any accelerometer data using the methods of this class. Accelerometer data recording is not supported on all devices.

## See Also

### Checking the Availability of Sensor Recording

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to record sensor data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

class func isAuthorizedForRecording() -> Bool

Returns a Boolean value indicating whether the app is authorized to record sensor data.

Deprecated

