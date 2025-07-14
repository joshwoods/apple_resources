

- AVFoundation
-  AVCaptureAudioPreviewOutput 

Class

# AVCaptureAudioPreviewOutput

A capture output that provides a preview of the captured audio.

macOS 10.7+

``` source
class AVCaptureAudioPreviewOutput
```

## Topics

### Creating Preview Output

init()

Creates an audio preview output object.

### Configuring the Output

var volume: Float

The output volume of the audio preview.

var outputDeviceUniqueID: String?

The unique identifier of the Core Audio output device to use for audio preview.

## Relationships

### Inherits From

- AVCaptureOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Capture preview

class AVCaptureVideoPreviewLayer

A Core Animation layer that displays video from a camera device.

