

- AVFAudio
- AVSpeechSynthesisProviderVoice
-  supportedLanguages 

Instance Property

# supportedLanguages

A list of BCP 47 codes that identify the languages a voice supports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var supportedLanguages: [String] { get }
```

## Discussion

These languages are what a voice supports — when given a multi-language phrase — without the need to switch voice. For example, if the primary language is `zh-CN`, and this value contains `zh-CN` and `en-US`, a synthesizer that receives a phrase with both languages would speak the entire phrase.

## See Also

### Inspecting a voice

var age: Int

The age of the voice, in years.

var gender: AVSpeechSynthesisVoiceGender

The gender of the voice.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

var identifier: String

The unique identifier for the voice.

var name: String

The localized name of the voice.

var primaryLanguages: [String]

A list of BCP 47 codes that identify the languages the synthesizer uses.

var version: String

The version of the voice.

var voiceSize: Int64

The size of the voice package on disk, in bytes.

