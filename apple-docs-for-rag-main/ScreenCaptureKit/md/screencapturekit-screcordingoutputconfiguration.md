

- ScreenCaptureKit
-  SCRecordingOutputConfiguration 

Class

# SCRecordingOutputConfiguration

Mac Catalyst 18.2+macOS 15.0+

``` source
class SCRecordingOutputConfiguration
```

## Topics

### Instance Properties

var availableOutputFileTypes: [AVFileType]

var availableVideoCodecTypes: [AVVideoCodecType]

var outputFileType: AVFileType

var outputURL: URL

var videoCodecType: AVVideoCodecType

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

### Creating a recording output

init(configuration: SCRecordingOutputConfiguration, delegate: any SCRecordingOutputDelegate)

protocol SCRecordingOutputDelegate

