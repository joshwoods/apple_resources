

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.MicrophoneMode 

Enumeration

# AVCaptureDevice.MicrophoneMode

Constants that define the available microphone modes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
enum MicrophoneMode
```

## Topics

### Microphone Modes

case standard

A mode that processes microphone audio with standard voice DSP.

case wideSpectrum

A mode that minimizes microphone audio processing to capture all sounds in the room.

case voiceIsolation

A mode that processes microphone audio to isolate the voice and attenuate other signals.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the Microphone Mode

class var activeMicrophoneMode: AVCaptureDevice.MicrophoneMode

The device’s active microphone mode.

class var preferredMicrophoneMode: AVCaptureDevice.MicrophoneMode

The microphone mode that the user selects in Control Center.

