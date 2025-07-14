

- AVFAudio
-  AVSpeechSynthesisVoiceGender 

Enumeration

# AVSpeechSynthesisVoiceGender

The gender for a voice.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum AVSpeechSynthesisVoiceGender
```

## Topics

### Voice genders

case unspecified

The nonspecific gender option.

case male

The male voice option.

case female

The female voice option.

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

enum AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

struct Traits

Traits that describe a voice.

