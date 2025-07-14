

- SensorKit
- SRSensorReader
-  startRecording() 

Instance Method

# startRecording()

Starts recording sensor data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func startRecording()
```

## Discussion

This function instructs the framework to start recording for this reader’s sensor. The framework records on this device and any paired devices. Call fetchDevices() to acquire the full list of devices on which the framework records.

The framework allows a sensor to be recorded simultaneously by multiple readers, either in the same app or across different apps on the same system. On multiple calls to this function, the framework just ensures that recording for the sensor is active.

Upon success, the framework calls the delegate’s sensorReaderWillStartRecording(_:) callback. Upon failure, the framework calls the delegate’s sensorReader(_:startRecordingFailedWithError:).

The reader must be authorized (see authorizationStatus) for this function to succeed.

## See Also

### Recording sensor data

func stopRecording()

Stops recording sensor data.

