

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.CommandDelimiterKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.CommandDelimiterKey

Keys for the command delimiters.

macOS 10.3–14.0Deprecated

``` source
struct CommandDelimiterKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use these keys in the commandDelimiter dictionary.

## Topics

### Delimiter Keys

static let prefix: NSSpeechSynthesizer.SpeechPropertyKey.CommandDelimiterKey

The command delimiter string that prefixes a command, by default, this is `[[`.

static let suffix: NSSpeechSynthesizer.SpeechPropertyKey.CommandDelimiterKey

The command delimiter string that suffixes a command,by default, this is `]]`.

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

