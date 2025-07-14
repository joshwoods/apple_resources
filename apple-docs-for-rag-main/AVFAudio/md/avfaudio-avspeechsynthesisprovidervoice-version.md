

- AVFAudio
- AVSpeechSynthesisProviderVoice
-  version 

Instance Property

# version

The version of the voice.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var version: String { get set }
```

## Discussion

This value is for your own tracking and doesn’t impact the behavior of the system.

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

var supportedLanguages: [String]

A list of BCP 47 codes that identify the languages a voice supports.

var voiceSize: Int64

The size of the voice package on disk, in bytes.

