

- ScreenCaptureKit
-  SCRecordingOutputDelegate 

Protocol

# SCRecordingOutputDelegate

Mac Catalyst 18.2+macOS 15.0+

``` source
protocol SCRecordingOutputDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func recordingOutput(SCRecordingOutput, didFailWithError: any Error)

func recordingOutputDidFinishRecording(SCRecordingOutput)

func recordingOutputDidStartRecording(SCRecordingOutput)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a recording output

init(configuration: SCRecordingOutputConfiguration, delegate: any SCRecordingOutputDelegate)

class SCRecordingOutputConfiguration

