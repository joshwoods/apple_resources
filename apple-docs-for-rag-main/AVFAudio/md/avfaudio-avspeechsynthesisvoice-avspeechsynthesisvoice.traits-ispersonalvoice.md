

- AVFAudio
- AVSpeechSynthesisVoice
- AVSpeechSynthesisVoice.Traits
-  isPersonalVoice 

Type Property

# isPersonalVoice

The trait that indicates a voice is a personal voice.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var isPersonalVoice: AVSpeechSynthesisVoice.Traits { get }
```

## Discussion

A user generates and owns a personal voice.

Note

The system only makes personal voices available when personalVoiceAuthorizationStatus is AVSpeechSynthesizer.PersonalVoiceAuthorizationStatus.authorized.

## See Also

### Inspecting a voice trait

static var isNoveltyVoice: AVSpeechSynthesisVoice.Traits

The trait that indicates a voice is a novelty voice.

