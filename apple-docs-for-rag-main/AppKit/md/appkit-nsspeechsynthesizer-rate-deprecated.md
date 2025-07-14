

- AppKit
- NSSpeechSynthesizer
-  rate Deprecated

Instance Property

# rate

The synthesizer’s speaking rate (words per minute).

macOS 10.5–14.0Deprecated

``` source
var rate: Float { get set }
```

## Discussion

The range of supported rates is not predefined by the Speech Synthesis framework; but the synthesizer may only respond to a limited range of speech rates. Average human speech occurs at a rate of 180 to 220 words per minute.

## See Also

### Configuring Speech Synthesizers

var usesFeedbackWindow: Bool

Indicates whether the receiver uses the speech feedback window.

Deprecated

func voice() -> NSSpeechSynthesizer.VoiceName?

Returns the identifier of the receiver’s current voice.

Deprecated

func setVoice(NSSpeechSynthesizer.VoiceName?) -> Bool

Sets the receiver’s current voice.

Deprecated

var volume: Float

The synthesizer’s speaking volume.

Deprecated

