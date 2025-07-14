

- AVFAudio
- AVSpeechUtterance
-  volume 

Instance Property

# volume

The volume the speech synthesizer uses when speaking the utterance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var volume: Float { get set }
```

## Discussion

Before enqueing the utterance, set this property to a value within the range of `0.0` for silent to `1.0` for loudest volume. The default value is `1.0`. Setting this after enqueing the utterance has no effect.

## See Also

### Configuring an utterance

var voice: AVSpeechSynthesisVoice?

The voice the speech synthesizer uses when speaking the utterance.

var pitchMultiplier: Float

The baseline pitch the speech synthesizer uses when speaking the utterance.

var prefersAssistiveTechnologySettings: Bool

A Boolean that specifies whether assistive technology settings take precedence over the property values of this utterance.

