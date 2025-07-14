

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.VoiceAttributeKey
-  supportedCharacters 

Type Property

# supportedCharacters

A list of Unicode character id ranges that define the Unicode characters supported by this voice.

macOS 10.5+

``` source
static let supportedCharacters: NSSpeechSynthesizer.VoiceAttributeKey
```

## Discussion

A dictionary containing two keys: “UnicodeCharBegin”, an integer value containing the beginning Unicode id of this range; and “UnicodeCharBegin”, an integer value containing the ending Unicode id of this range. The synthesizer converts or ignores any characters not contained in the range of supported characters.

Some voices may not provide this attribute.

## See Also

### Voice Attribute Keys

static let identifier: NSSpeechSynthesizer.VoiceAttributeKey

A unique string identifying the voice. The identifiers of the system voices are listed in `Listing 1`.

Deprecated

static let name: NSSpeechSynthesizer.VoiceAttributeKey

The name of the voice suitable for display. An `NSString`.

Deprecated

static let age: NSSpeechSynthesizer.VoiceAttributeKey

The perceived age (in years) of the voice. An `NSString`

Deprecated

static let gender: NSSpeechSynthesizer.VoiceAttributeKey

The perceived gender of the voice. The supported values are listed in `Voice Gender Keys`. An `NSString`

Deprecated

static let demoText: NSSpeechSynthesizer.VoiceAttributeKey

A demonstration string to speak. An `NSString`

Deprecated

static let localeIdentifier: NSSpeechSynthesizer.VoiceAttributeKey

The language of the voice. An `NSString`

static let individuallySpokenCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters that can be spoken in character-by-character mode by this voice.

