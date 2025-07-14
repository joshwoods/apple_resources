

- WatchKit
-  WKAudioRecorderPreset 

Enumeration

# WKAudioRecorderPreset

Constants indicating the quality of audio recordings.

watchOS 2.0+

``` source
enum WKAudioRecorderPreset
```

## Topics

### Constants

case narrowBandSpeech

Audio quality suitable for basic speech recording. This preset records audio with an 8 kHz sampling rate using either the LPCM 128 kbps or AAC 24 kbps format.

case wideBandSpeech

Audio quality suitable for higher fidelity speech recording. This preset records audio with a 16 kHz sampling rate using either the LPCM 256 kbps or AAC 32 kbps format.

case highQualityAudio

A high-quality audio recording. This preset records audio with a 44.1 kHz sampling rate using either the LPCM 705.6 kbps or AAC 96 kbps format.

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

### Presenting video and audio interfaces

func presentMediaPlayerController(with: URL, options: [AnyHashable : Any]?, completion: (Bool, TimeInterval, (any Error)?) -> Void)

Displays a modal interface for playing the specified media file.

Media Player Options

Keys indicating media playback options.

func dismissMediaPlayerController()

Dismisses the media interface controller.

func presentAudioRecorderController(withOutputURL: URL, preset: WKAudioRecorderPreset, options: [AnyHashable : Any]?, completion: (Bool, (any Error)?) -> Void)

Display a standard interface for recording audio from the user’s Apple Watch.

Audio Recording Options

Options to specify when recording audio.

func dismissAudioRecorderController()

Dismisses the audio recording interface controller.

