

- ScreenCaptureKit
-  SCRecordingOutput 

Class

# SCRecordingOutput

Mac Catalyst 18.2+macOS 15.0+

``` source
class SCRecordingOutput
```

## Topics

### Creating a recording output

init(configuration: SCRecordingOutputConfiguration, delegate: any SCRecordingOutputDelegate)

class SCRecordingOutputConfiguration

protocol SCRecordingOutputDelegate

### Configuring the recording output

var recordedDuration: CMTime

var recordedFileSize: Int

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

### Adding and removing recording output

func addRecordingOutput(SCRecordingOutput) throws

func removeRecordingOutput(SCRecordingOutput) throws

