

- AVFAudio
- AVSpeechUtterance
-  voice 

Instance Property

# voice

The voice the speech synthesizer uses when speaking the utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var voice: AVSpeechSynthesisVoice? { get set }
```

## Discussion

If you don’t specify a voice, the speech synthesizer uses the system’s default voice to speak the utterance.

## See Also

### Configuring an utterance

var pitchMultiplier: Float

The baseline pitch the speech synthesizer uses when speaking the utterance.

var volume: Float

The volume the speech synthesizer uses when speaking the utterance.

var prefersAssistiveTechnologySettings: Bool

A Boolean that specifies whether assistive technology settings take precedence over the property values of this utterance.

