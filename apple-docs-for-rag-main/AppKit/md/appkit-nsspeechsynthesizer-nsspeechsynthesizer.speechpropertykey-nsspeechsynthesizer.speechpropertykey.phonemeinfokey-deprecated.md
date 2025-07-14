

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

Keys for the speech phoneme information.

macOS 10.3–14.0Deprecated

``` source
struct PhonemeInfoKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use these keys in the phonemeSymbols dictionary.

## Topics

### Phoneme Info Keys

static let example: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

An example word that illustrates the use of the phoneme.

static let hiliteEnd: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

The character offset into the example word that identifies the location of the end of the phoneme.

static let hiliteStart: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

The character offset into the example word that identifies the location of the beginning of the phoneme.

static let opcode: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

NSNumber

static let symbol: NSSpeechSynthesizer.SpeechPropertyKey.PhonemeInfoKey

The symbol used to represent the phoneme.

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

struct DictionaryKey

These constants identify key-value pairs used to add vocabulary to the dictionary using addSpeechDictionary(_:).

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

struct StatusKey

Keys for the speech synthesizier status.

Deprecated

struct SynthesizerInfoKey

Keys for the speech synthesizier information.

Deprecated

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

Deprecated

