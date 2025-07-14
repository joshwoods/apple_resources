

- AVFoundation
-  AVCaptureMultichannelAudioMode 

Enumeration

# AVCaptureMultichannelAudioMode

Constants that indicate the modes of multichannel audio.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
enum AVCaptureMultichannelAudioMode
```

## Topics

### Modes

case none

A mode that indicates there’s no multichannel audio.

case stereo

A mode that indicates the recording uses stereo audio.

case firstOrderAmbisonics

An audio mode that indicates the recording uses first-order ambisonics.

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

### Configuring audio properties

func isMultichannelAudioModeSupported(AVCaptureMultichannelAudioMode) -> Bool

A Boolean value that indicates whether the input supports the specified multichannel audio mode.

var multichannelAudioMode: AVCaptureMultichannelAudioMode

The multichannel audio mode to apply when recording audio.

