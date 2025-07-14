

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

Keys that identify errors that may occur during speech synthesis.

macOS 10.3–14.0Deprecated

``` source
struct ErrorKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use these keys in the errors dictionary.

## Topics

### Type Properties

static let count: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The number of errors that have occurred in processing the current text string, since the last call to object(forProperty:) with the errors property. An `NSNumber`

static let newestCharacterOffset: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The position in the text string of the most recent error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`.

static let newestCode: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The error code of the most recent error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

static let oldestCharacterOffset: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The position in the text string of the first error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

static let oldestCode: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The error code of the first error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

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

