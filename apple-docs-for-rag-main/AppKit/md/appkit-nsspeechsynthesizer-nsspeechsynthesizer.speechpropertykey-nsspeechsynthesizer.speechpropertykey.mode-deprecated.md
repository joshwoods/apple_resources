

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.Mode Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.Mode

Keys for the speaking mode.

macOS 10.3–14.0Deprecated

``` source
struct Mode
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use these keys in the inputMode, characterMode, and numberMode dictionaries.

## Topics

### Type Properties

static let literal: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that each digit or character is spoken literally (so that 12 is spoken as “one, two”, or the word “cat” is spoken as “C A T”).

static let normal: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that the synthesizer assembles digits into numbers (so that 12 is spoken as “twelve”) and text into words.

static let phoneme: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that the synthesizer is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

static let text: NSSpeechSynthesizer.SpeechPropertyKey.Mode

Indicates that the synthesizer is in text-processing mode.

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

