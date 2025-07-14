

- AVFAudio
-  AVSpeechSynthesisVoiceQuality 

Enumeration

# AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum AVSpeechSynthesisVoiceQuality
```

## Topics

### Voice qualities

case `default`

A basic quality voice that’s available on the device by default.

case enhanced

An enhanced quality voice that you must download to use.

case premium

A premium quality voice that you must download to use.

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

### Inspecting voices

var identifier: String

The unique identifier of a voice.

var name: String

The name of a voice.

var quality: AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

var gender: AVSpeechSynthesisVoiceGender

The gender for a voice.

var voiceTraits: AVSpeechSynthesisVoice.Traits

The traits of a voice.

var audioFileSettings: [String : Any]

A dictionary that contains audio file settings.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

struct Traits

Traits that describe a voice.

