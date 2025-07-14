

- AppKit
- NSSpeechSynthesizer
-  volume Deprecated

Instance Property

# volume

The synthesizer’s speaking volume.

macOS 10.5–14.0Deprecated

``` source
var volume: Float { get set }
```

## Discussion

Volumes are expressed in floating-point units ranging from 0.0 through 1.0. A value of 0.0 corresponds to silence, and a value of 1.0 corresponds to the maximum possible volume. Volume units lie on a scale that is linear with amplitude or voltage. A doubling of perceived loudness corresponds to a doubling of the volume. Setting a value outside this range is undefined.

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

var rate: Float

The synthesizer’s speaking rate (words per minute).

Deprecated

