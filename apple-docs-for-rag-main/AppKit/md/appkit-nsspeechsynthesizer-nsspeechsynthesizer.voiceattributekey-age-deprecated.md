

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.VoiceAttributeKey
-  age Deprecated

Type Property

# age

The perceived age (in years) of the voice. An `NSString`

macOS 10.3–14.0Deprecated

``` source
static let age: NSSpeechSynthesizer.VoiceAttributeKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## See Also

### Voice Attribute Keys

static let identifier: NSSpeechSynthesizer.VoiceAttributeKey

A unique string identifying the voice. The identifiers of the system voices are listed in `Listing 1`.

Deprecated

static let name: NSSpeechSynthesizer.VoiceAttributeKey

The name of the voice suitable for display. An `NSString`.

Deprecated

static let gender: NSSpeechSynthesizer.VoiceAttributeKey

The perceived gender of the voice. The supported values are listed in `Voice Gender Keys`. An `NSString`

Deprecated

static let demoText: NSSpeechSynthesizer.VoiceAttributeKey

A demonstration string to speak. An `NSString`

Deprecated

static let localeIdentifier: NSSpeechSynthesizer.VoiceAttributeKey

The language of the voice. An `NSString`

static let supportedCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters supported by this voice.

static let individuallySpokenCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters that can be spoken in character-by-character mode by this voice.

