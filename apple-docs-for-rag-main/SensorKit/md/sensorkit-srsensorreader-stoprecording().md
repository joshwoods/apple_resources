

- SensorKit
- SRSensorReader
-  stopRecording() 

Instance Method

# stopRecording()

Stops recording sensor data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func stopRecording()
```

## Discussion

This function requests that the framework stop recording for this reader’s sensor. The framework records on this device and any paired devices. Call fetchDevices() to get acquire the full list of devices on which the framework records.

The framework allows a sensor to be recorded simultaneously by multiple readers, either in the same app, or across different apps on the same system. As a result, this function signifies that the caller relinquishes interest in recording the reader’s sensor.

Upon success, the framework calls the delegate’s sensorReaderDidStopRecording(_:) callback. Upon failure, the framework calls the delegate’s sensorReader(_:stopRecordingFailedWithError:).

The reader must be authorized (see authorizationStatus) for this function to succeed.

## See Also

### Recording sensor data

func startRecording()

Starts recording sensor data.

