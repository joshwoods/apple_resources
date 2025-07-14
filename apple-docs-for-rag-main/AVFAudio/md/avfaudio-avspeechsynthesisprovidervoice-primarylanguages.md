

- AVFAudio
- AVSpeechSynthesisProviderVoice
-  primaryLanguages 

Instance Property

# primaryLanguages

A list of BCP 47 codes that identify the languages the synthesizer uses.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var primaryLanguages: [String] { get }
```

## Discussion

These languages are what a voice primarily supports. For example, if the primary language is `zh-CN —` with no additional supportedLanguages — the system may switch voices to speak a phrase that contains other languages. Changing voices depends on user preferences and what accessibility feature is using the voice.

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

var supportedLanguages: [String]

A list of BCP 47 codes that identify the languages a voice supports.

var version: String

The version of the voice.

var voiceSize: Int64

The size of the voice package on disk, in bytes.

