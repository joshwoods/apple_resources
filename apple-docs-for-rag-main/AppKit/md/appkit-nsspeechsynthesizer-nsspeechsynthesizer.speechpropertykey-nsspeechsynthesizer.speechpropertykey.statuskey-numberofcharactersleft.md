

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
- NSSpeechSynthesizer.SpeechPropertyKey.StatusKey
-  numberOfCharactersLeft 

Type Property

# numberOfCharactersLeft

The number of characters left in the input string of text.

macOS 10.5+

``` source
static let numberOfCharactersLeft: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey
```

## Discussion

When the value of this key is zero, you can destroy the input string.

## See Also

### Status Keys

static let outputBusy: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates whether the synthesizer is currently producing speech.

static let outputPaused: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates whether speech output in the synthesizer has been paused by sending the message pauseSpeaking(at:).

static let phonemeCode: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates that the synthesizer is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

