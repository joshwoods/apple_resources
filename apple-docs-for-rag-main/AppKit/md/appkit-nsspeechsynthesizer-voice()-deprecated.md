

- AppKit
- NSSpeechSynthesizer
-  voice() Deprecated

Instance Method

# voice()

Returns the identifier of the receiver’s current voice.

macOS 10.3–14.0Deprecated

``` source
func voice() -> NSSpeechSynthesizer.VoiceName?
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Return Value

Identifier of the receiver’s current voice.

## See Also

### Configuring Speech Synthesizers

var usesFeedbackWindow: Bool

Indicates whether the receiver uses the speech feedback window.

Deprecated

func setVoice(NSSpeechSynthesizer.VoiceName?) -> Bool

Sets the receiver’s current voice.

Deprecated

var rate: Float

The synthesizer’s speaking rate (words per minute).

Deprecated

var volume: Float

The synthesizer’s speaking volume.

Deprecated

