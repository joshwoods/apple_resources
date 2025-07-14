

- AVFAudio
- AVSpeechSynthesisVoice
-  AVSpeechSynthesisVoice.Traits 

Structure

# AVSpeechSynthesisVoice.Traits

Traits that describe a voice.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Traits
```

## Topics

### Creating a voice trait

init(rawValue: UInt)

Creates a voice trait with the corresponding integer that you specify.

### Inspecting a voice trait

static var isNoveltyVoice: AVSpeechSynthesisVoice.Traits

The trait that indicates a voice is a novelty voice.

static var isPersonalVoice: AVSpeechSynthesisVoice.Traits

The trait that indicates a voice is a personal voice.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

