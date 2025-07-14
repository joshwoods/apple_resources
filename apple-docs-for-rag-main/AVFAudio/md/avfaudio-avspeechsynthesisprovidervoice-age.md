

- AVFAudio
- AVSpeechSynthesisProviderVoice
-  age 

Instance Property

# age

The age of the voice, in years.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var age: Int { get set }
```

## Discussion

The system treats this value as a personality trait and defaults to `0`.

## See Also

### Inspecting a voice

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

var supportedLanguages: [String]

A list of BCP 47 codes that identify the languages a voice supports.

var version: String

The version of the voice.

var voiceSize: Int64

The size of the voice package on disk, in bytes.

