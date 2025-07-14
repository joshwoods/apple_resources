

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:stopRecordingFailedWithError:) 

Instance Method

# sensorReader(\_:stopRecordingFailedWithError:)

Provides the delegate with a reason when the reader fails to stop recording.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    stopRecordingFailedWithError error: any Error
)
```

## Parameters 

`reader`  

The sensor reader that failed to stop recording.

`error`  

An object that describes the cause of failure.

## See Also

### Recording Data

func sensorReaderWillStartRecording(SRSensorReader)

Notifies the delegate when a reader starts recording.

func sensorReader(SRSensorReader, startRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to record.

func sensorReaderDidStopRecording(SRSensorReader)

Notifies the delegate when a reader stops recording.

