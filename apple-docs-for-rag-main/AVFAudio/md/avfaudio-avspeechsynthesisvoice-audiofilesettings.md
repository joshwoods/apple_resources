

- AVFAudio
- AVSpeechSynthesisVoice
-  audioFileSettings 

Instance Property

# audioFileSettings

A dictionary that contains audio file settings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var audioFileSettings: [String : Any] { get }
```

## Discussion

If you want to generate speech and save it as an audio file to share or play later, use this dictionary to create an AVAudioFile instance and pass it as the `settings` parameter.

You can determine the AVAudioCommonFormat and interleaved properties of a voice from this dictionary. The format of this dictionary matches the data that AVSpeechSynthesizer.BufferCallback provides for the same voice.

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

enum AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

struct Traits

Traits that describe a voice.

