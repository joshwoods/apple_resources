

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.VoiceAttributeKey
-  localeIdentifier 

Type Property

# localeIdentifier

The language of the voice. An `NSString`

macOS 10.5+

``` source
static let localeIdentifier: NSSpeechSynthesizer.VoiceAttributeKey
```

## Discussion

The canonical locale identifier string describing the voice’s locale. A locale is generally composed of three pieces of ordered information: a language code, a region code, and a variant code. Refer to documentation about the NSLocale class or Internationalization and Localization Guide for more information.

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

static let supportedCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters supported by this voice.

static let individuallySpokenCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters that can be spoken in character-by-character mode by this voice.

