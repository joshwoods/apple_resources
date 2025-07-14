

- Core Motion
-  CMSensorRecorder 

Class

# CMSensorRecorder

An object that gathers and retrieves accelerometer data from a device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class CMSensorRecorder
```

## Mentioned in 

Getting movement disorder symptom data

## Overview

Use a sensor recorder to initiate the gathering of accelerometer data. Later, use the sensor recorder to fetch the recorded data so you can analyze it. You might use the recorded data to assess specific types of motion and incorporate the results into your app.

To use a sensor recorder, create an instance of this class and call the recordAccelerometer(forDuration:) method to begin recording data. You do not need to stop the recording process explicitly. The system stops recording automatically when the specified time expires and no other apps extend the recording time. The following example shows how to record 20 minutes worth of accelerometer data:

- Swift
- Objective-C

```
if CMSensorRecorder.isAccelerometerRecordingAvailable() {
    let recorder = CMSensorRecorder()
    recorder.recordAccelerometerForDuration(20 * 60)  // Record for 20 minutes
}
```

```
if ([CMSensorRecorder isAccelerometerRecordingAvailable]) {
   CMSensorRecorder* recorder = [[CMSensorRecorder alloc] init];
   [recorder recordAccelerometerForDuration:(20 * 60)]; // Record for 20 minutes
}
```

Important

To use this API, you must include the NSMotionUsageDescription key in your app’s `Info.plist` file and provide a usage description string for this key. The usage description appears in the prompt that the user must accept the first time the system asks the user to access motion data for your app. If you don’t include a usage description string, your app crashes when you call this API.

## Topics

### Checking the Availability of Sensor Recording

class func isAccelerometerRecordingAvailable() -> Bool

Returns a Boolean value indicating whether accelerometer recording is supported on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to record sensor data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

class func isAuthorizedForRecording() -> Bool

Returns a Boolean value indicating whether the app is authorized to record sensor data.

Deprecated

### Recording Accelerometer Data

func recordAccelerometer(forDuration: TimeInterval)

Begins recording accelerometer data for the specified period of time.

### Retrieving Past Accelerometer Data

func accelerometerData(from: Date, to: Date) -> CMSensorDataList?

Retrieves the accelerometer data collected between the specified dates.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accelerometers

Getting raw accelerometer events

Retrieve data from the onboard accelerometers.

class CMAccelerometerData

A data sample from the device’s three accelerometers.

class CMRecordedAccelerometerData

A single piece of accelerometer data that was recorded by the device.

class CMSensorDataList

A list of the accelerometer data recorded by the system.

