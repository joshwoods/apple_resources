

- AppKit
- NSSpeechSynthesizer
-  usesFeedbackWindow Deprecated

Instance Property

# usesFeedbackWindow

Indicates whether the receiver uses the speech feedback window.

macOS 10.3–14.0Deprecated

``` source
var usesFeedbackWindow: Bool { get set }
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

true when the receiver uses the speech feedback window, false otherwise.

See the class description for details on the `UsesFeedbackWindow` attribute.

Important

The delegate only receives the speechSynthesizer(_:didFinishSpeaking:) message when speaking occurs through the feedback window.

## See Also

### Configuring Speech Synthesizers

func voice() -> NSSpeechSynthesizer.VoiceName?

Returns the identifier of the receiver’s current voice.

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

