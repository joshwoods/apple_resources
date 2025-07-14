

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
- NSSpeechSynthesizer.SpeechPropertyKey.Mode
-  normal 

Type Property

# normal

Indicates that the synthesizer assembles digits into numbers (so that 12 is spoken as “twelve”) and text into words.

macOS 10.5+

``` source
static let normal: NSSpeechSynthesizer.SpeechPropertyKey.Mode
```

## See Also

### Type Properties

static let literal: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that each digit or character is spoken literally (so that 12 is spoken as “one, two”, or the word “cat” is spoken as “C A T”).

static let phoneme: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that the synthesizer is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

static let text: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that the synthesizer is in text-processing mode.

