

- AVFAudio
- AVSpeechSynthesisProviderRequest
-  ssmlRepresentation 

Instance Property

# ssmlRepresentation

The description of the text to synthesize.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var ssmlRepresentation: String { get }
```

## Discussion

The Speech Synthesis Markup Language describes the speech synthesis attributes for the customization of pitch, rate, intonation, and more.

## See Also

### Inspecting a request

var voice: AVSpeechSynthesisProviderVoice

The voice to use in the speech request.

class AVSpeechSynthesisProviderVoice

An object that represents a voice that an audio unit provides to its host.

