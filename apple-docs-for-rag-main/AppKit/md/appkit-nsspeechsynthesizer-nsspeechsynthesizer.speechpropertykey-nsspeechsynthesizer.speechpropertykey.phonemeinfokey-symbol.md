

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
- NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey
-  symbol 

Type Property

# symbol

The symbol used to represent the phoneme.

macOS 10.5+

``` source
static let symbol: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey
```

## Discussion

The symbol does not necessarily have a phonetic connection to the phoneme, but might simply be an abstract textual representation of it.

## See Also

### Phoneme Info Keys

static let example: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

An example word that illustrates the use of the phoneme.

static let hiliteEnd: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

The character offset into the example word that identifies the location of the end of the phoneme.

static let hiliteStart: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

The character offset into the example word that identifies the location of the beginning of the phoneme.

static let opcode: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

NSNumber

