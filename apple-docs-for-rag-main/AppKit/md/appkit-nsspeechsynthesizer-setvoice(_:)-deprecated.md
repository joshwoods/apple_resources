

- AppKit
- NSSpeechSynthesizer
-  setVoice(\_:) Deprecated

Instance Method

# setVoice(\_:)

Sets the receiver’s current voice.

macOS 10.3–14.0Deprecated

``` source
func setVoice(_ voice: NSSpeechSynthesizer.VoiceName?) -> Bool
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`voice`  

Identifier of the voice to set at the receiver’s current voice. When `nil`, the receiver sets the default voice as its current voice.

## Return Value

true when the receiver is not currently synthesizing speech and the current voice is set successfully, false otherwise.

## See Also

### Related Documentation

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

Deprecated

### Configuring Speech Synthesizers

var usesFeedbackWindow: Bool

Indicates whether the receiver uses the speech feedback window.

Deprecated

func voice() -> NSSpeechSynthesizer.VoiceName?

Returns the identifier of the receiver’s current voice.

Deprecated

var rate: Float

The synthesizer’s speaking rate (words per minute).

Deprecated

var volume: Float

The synthesizer’s speaking volume.

Deprecated

