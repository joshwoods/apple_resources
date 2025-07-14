

- AppKit
- NSSpeechSynthesizer
-  NSSpeechSynthesizer.DictionaryKey Deprecated

Structure

# NSSpeechSynthesizer.DictionaryKey

These constants identify key-value pairs used to add vocabulary to the dictionary using addSpeechDictionary(_:).

macOS 10.3–14.0Deprecated

``` source
struct DictionaryKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Topics

### Type Properties

static let abbreviations: NSSpeechSynthesizer.DictionaryKey

An array of dictionary objects containing the keys entrySpelling and entryPhonemes.

static let entryPhonemes: NSSpeechSynthesizer.DictionaryKey

The phonemic representation of an entry. An `NSString`.

static let entrySpelling: NSSpeechSynthesizer.DictionaryKey

The spelling of an entry. An `NSString`.

static let localeIdentifier: NSSpeechSynthesizer.DictionaryKey

The canonical locale identifier string describing the dictionary’s locale. A locale is generally composed of three pieces of ordered information: a language code, a region code, and a variant code. Refer to documentation about NSLocale or Internationalization and Localization Guide for more information

static let modificationDate: NSSpeechSynthesizer.DictionaryKey

A string representation of the dictionary’s last modification date in the international format (YYYY-MM-DD HH:MM:SS ±HHMM). If the same word appears across multiple dictionaries, the one from the dictionary with the most recent date will be used.

static let pronunciations: NSSpeechSynthesizer.DictionaryKey

An array of dictionary objects containing the keys entrySpelling and entryPhonemes.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Speech Attributes

func addSpeechDictionary([NSSpeechSynthesizer.DictionaryKey : Any])

Registers the given speech dictionary with the receiver.

Deprecated

func object(forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws -> Any

Provides the value of a receiver’s property.

Deprecated

func setObject(Any?, forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws

Specifies the value of a receiver’s property.

Deprecated

struct SpeechPropertyKey

These constants are used with setObject(_:forProperty:) and object(forProperty:) to get or set the characteristics of a synthesizer.

Deprecated

struct CommandDelimiterKey

Keys for the command delimiters.

Deprecated

struct ErrorKey

Keys that identify errors that may occur during speech synthesis.

Deprecated

struct Mode

Keys for the speaking mode.

Deprecated

struct PhonemeInfoKey

Keys for the speech phoneme information.

Deprecated

struct StatusKey

Keys for the speech synthesizier status.

Deprecated

struct SynthesizerInfoKey

Keys for the speech synthesizier information.

Deprecated

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

Deprecated

