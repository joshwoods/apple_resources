

- AVFAudio
- AVSpeechSynthesisVoice
-  voiceTraits 

Instance Property

# voiceTraits

The traits of a voice.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var voiceTraits: AVSpeechSynthesisVoice.Traits { get }
```

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

var audioFileSettings: [String : Any]

A dictionary that contains audio file settings.

enum AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

struct Traits

Traits that describe a voice.

