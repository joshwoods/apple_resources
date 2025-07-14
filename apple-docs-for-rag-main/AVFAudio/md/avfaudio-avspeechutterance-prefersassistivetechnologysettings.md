

- AVFAudio
- AVSpeechUtterance
-  prefersAssistiveTechnologySettings 

Instance Property

# prefersAssistiveTechnologySettings

A Boolean that specifies whether assistive technology settings take precedence over the property values of this utterance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var prefersAssistiveTechnologySettings: Bool { get set }
```

## Discussion

If this property is `true`, but no assistive technology, such as VoiceOver, is on, the speech synthesizer uses the utterance property values.

## See Also

### Configuring an utterance

var voice: AVSpeechSynthesisVoice?

The voice the speech synthesizer uses when speaking the utterance.

var pitchMultiplier: Float

The baseline pitch the speech synthesizer uses when speaking the utterance.

var volume: Float

The volume the speech synthesizer uses when speaking the utterance.

