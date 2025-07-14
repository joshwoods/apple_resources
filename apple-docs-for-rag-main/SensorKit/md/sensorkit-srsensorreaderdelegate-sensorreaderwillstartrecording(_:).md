

- SensorKit
- SRSensorReaderDelegate
-  sensorReaderWillStartRecording(\_:) 

Instance Method

# sensorReaderWillStartRecording(\_:)

Notifies the delegate when a reader starts recording.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func sensorReaderWillStartRecording(_ reader: SRSensorReader)
```

## Parameters 

`reader`  

The reader that stopped recording.

## See Also

### Recording Data

func sensorReader(SRSensorReader, startRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to record.

func sensorReaderDidStopRecording(SRSensorReader)

Notifies the delegate when a reader stops recording.

func sensorReader(SRSensorReader, stopRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to stop recording.

