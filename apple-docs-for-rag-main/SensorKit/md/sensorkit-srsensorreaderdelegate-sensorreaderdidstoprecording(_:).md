

- SensorKit
- SRSensorReaderDelegate
-  sensorReaderDidStopRecording(\_:) 

Instance Method

# sensorReaderDidStopRecording(\_:)

Notifies the delegate when a reader stops recording.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReaderDidStopRecording(_ reader: SRSensorReader)
```

## Parameters 

`reader`  

The reader that stopped recording.

## See Also

### Recording Data

func sensorReaderWillStartRecording(SRSensorReader)

Notifies the delegate when a reader starts recording.

func sensorReader(SRSensorReader, startRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to record.

func sensorReader(SRSensorReader, stopRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to stop recording.

