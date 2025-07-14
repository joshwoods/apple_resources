

- AVFAudio
- AVSpeechSynthesisProviderAudioUnit
-  speechVoices 

Instance Property

# speechVoices

A list of voices the audio unit provides to the system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var speechVoices: [AVSpeechSynthesisProviderVoice] { get set }
```

## Discussion

The list of voices that a user selects through Settings. Speech synthesizer audio unit extensions must provide this list. Override the getter to perform complex fetches that provide a dynamic list of voices.

## See Also

### Getting and setting voices

class AVSpeechSynthesisProviderVoice

An object that represents a voice that an audio unit provides to its host.

