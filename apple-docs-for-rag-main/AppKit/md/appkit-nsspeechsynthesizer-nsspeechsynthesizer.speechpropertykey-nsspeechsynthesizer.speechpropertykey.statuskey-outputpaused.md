

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
- NSSpeechSynthesizer.SpeechPropertyKey.StatusKey
-  outputPaused 

Type Property

# outputPaused

Indicates whether speech output in the synthesizer has been paused by sending the message pauseSpeaking(at:).

macOS 10.5+

``` source
static let outputPaused: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey
```

## See Also

### Status Keys

static let numberOfCharactersLeft: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

The number of characters left in the input string of text.

static let outputBusy: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates whether the synthesizer is currently producing speech.

static let phonemeCode: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates that the synthesizer is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

