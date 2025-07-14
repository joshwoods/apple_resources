

- AVFoundation
- AVCaptureDevice
-  preferredMicrophoneMode 

Type Property

# preferredMicrophoneMode

The microphone mode that the user selects in Control Center.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
class var preferredMicrophoneMode: AVCaptureDevice.MicrophoneMode { get }
```

## Discussion

Use key-value observing to monitor the user’s microphone mode selection.

## See Also

### Inspecting the Microphone Mode

class var activeMicrophoneMode: AVCaptureDevice.MicrophoneMode

The device’s active microphone mode.

enum MicrophoneMode

Constants that define the available microphone modes.

