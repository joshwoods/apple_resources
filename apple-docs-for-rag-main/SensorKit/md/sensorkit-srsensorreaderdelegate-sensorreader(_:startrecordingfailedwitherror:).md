

- SensorKit
- SRSensorReaderDelegate
-  sensorReader(\_:startRecordingFailedWithError:) 

Instance Method

# sensorReader(\_:startRecordingFailedWithError:)

Provides the delegate with a reason when the reader fails to record.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReader(
    _ reader: SRSensorReader,
    startRecordingFailedWithError error: any Error
)
```

## Parameters 

`reader`  

The sensor reader that failed to start recording.

`error`  

An object that describes the cause of failure.

## See Also

### Recording Data

func sensorReaderWillStartRecording(SRSensorReader)

Notifies the delegate when a reader starts recording.

func sensorReaderDidStopRecording(SRSensorReader)

Notifies the delegate when a reader stops recording.

func sensorReader(SRSensorReader, stopRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to stop recording.

