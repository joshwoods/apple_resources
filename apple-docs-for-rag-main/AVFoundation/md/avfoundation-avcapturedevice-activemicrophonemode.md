

- AVFoundation
- AVCaptureDevice
-  activeMicrophoneMode 

Type Property

# activeMicrophoneMode

The device’s active microphone mode.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
class var activeMicrophoneMode: AVCaptureDevice.MicrophoneMode { get }
```

## Discussion

The value may differ from the value of the preferredMicrophoneMode property if the app’s active audio route doesn’t support the mode.

This property is key-value observable.

## See Also

### Inspecting the Microphone Mode

class var preferredMicrophoneMode: AVCaptureDevice.MicrophoneMode

The microphone mode that the user selects in Control Center.

enum MicrophoneMode

Constants that define the available microphone modes.

