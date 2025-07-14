

- AppKit
- NSSpeechSynthesizer
-  NSSpeechSynthesizer.VoiceAttributeKey Deprecated

Structure

# NSSpeechSynthesizer.VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

macOS 10.3–14.0Deprecated

``` source
struct VoiceAttributeKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Overview

The following are the identifiers of the macOS system voices (defined in `/System/Library/Speech/Voices`):

```
com.apple.speech.synthesis.voice.Agnes
com.apple.speech.synthesis.voice.Albert
com.apple.speech.synthesis.voice.Alex
com.apple.speech.synthesis.voice.BadNews
com.apple.speech.synthesis.voice.Bahh
com.apple.speech.synthesis.voice.Bells
com.apple.speech.synthesis.voice.Boing
com.apple.speech.synthesis.voice.Bruce
com.apple.speech.synthesis.voice.Bubbles
com.apple.speech.synthesis.voice.Cellos
com.apple.speech.synthesis.voice.Deranged
com.apple.speech.synthesis.voice.Fred
com.apple.speech.synthesis.voice.GoodNews
com.apple.speech.synthesis.voice.Hysterical
com.apple.speech.synthesis.voice.Junior
com.apple.speech.synthesis.voice.Kathy
com.apple.speech.synthesis.voice.Organ
com.apple.speech.synthesis.voice.Princess
com.apple.speech.synthesis.voice.Ralph
com.apple.speech.synthesis.voice.Trinoids
com.apple.speech.synthesis.voice.Vicki
com.apple.speech.synthesis.voice.Victoria
com.apple.speech.synthesis.voice.Whisper
com.apple.speech.synthesis.voice.Zarvox
```

## Topics

### Voice Attribute Keys

static let identifier: NSSpeechSynthesizer.VoiceAttributeKey

A unique string identifying the voice. The identifiers of the system voices are listed in `Listing 1`.

static let name: NSSpeechSynthesizer.VoiceAttributeKey

The name of the voice suitable for display. An `NSString`.

static let age: NSSpeechSynthesizer.VoiceAttributeKey

The perceived age (in years) of the voice. An `NSString`

static let gender: NSSpeechSynthesizer.VoiceAttributeKey

The perceived gender of the voice. The supported values are listed in `Voice Gender Keys`. An `NSString`

static let demoText: NSSpeechSynthesizer.VoiceAttributeKey

A demonstration string to speak. An `NSString`

static let localeIdentifier: NSSpeechSynthesizer.VoiceAttributeKey

The language of the voice. An `NSString`

static let supportedCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters supported by this voice.

static let individuallySpokenCharacters: NSSpeechSynthesizer.VoiceAttributeKey

A list of Unicode character id ranges that define the Unicode characters that can be spoken in character-by-character mode by this voice.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Speech Synthesizer Information

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

Deprecated

class func attributes(forVoice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]

Provides the attribute dictionary of a voice.

Deprecated

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

Deprecated

struct VoiceNameDeprecated

