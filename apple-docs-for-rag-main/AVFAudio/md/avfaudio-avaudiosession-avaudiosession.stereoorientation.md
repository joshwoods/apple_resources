

- AVFAudio
- AVAudioSession
-  AVAudioSession.StereoOrientation 

Enumeration

# AVAudioSession.StereoOrientation

Constants that define the supported stereo orientations.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum StereoOrientation
```

## Topics

### Stereo Orientations

case none

The audio session isn’t configured for stereo recording.

case portrait

Audio capture should be vertically oriented, with the USB-C or Lightning connector on the bottom.

case portraitUpsideDown

Audio capture should be vertically oriented, with the USB-C or Lightning connector on the top.

case landscapeRight

Audio capture should be horizontally oriented, with the USB-C or Lightning connector on the right.

case landscapeLeft

Audio capture should be horizontally oriented, with the USB-C or Lightning connector on the left.

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

### Enabling stereo recording

var inputOrientation: AVAudioSession.StereoOrientation

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

var preferredInputOrientation: AVAudioSession.StereoOrientation

The audio session’s preferred stereo input orientation.

func setPreferredInputOrientation(AVAudioSession.StereoOrientation) throws

Sets the audio session’s preferred stereo input orientation.

