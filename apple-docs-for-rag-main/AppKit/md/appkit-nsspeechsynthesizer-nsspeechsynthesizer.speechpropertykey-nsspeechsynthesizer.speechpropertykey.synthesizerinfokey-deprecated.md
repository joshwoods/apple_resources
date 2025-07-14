

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.SynthesizerInfoKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.SynthesizerInfoKey

Keys for the speech synthesizier information.

macOS 10.3–14.0Deprecated

``` source
struct SynthesizerInfoKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use constants as keys for the synthesizerInfo dictionary.

## Topics

### Synthesizer Info Keys

static let identifier: NSSpeechSynthesizer.SpeechPropertyKey.SynthesizerInfoKey

The identifier of the speech synthesizer.

static let version: NSSpeechSynthesizer.SpeechPropertyKey.SynthesizerInfoKey

The version of the speech synthesizer.

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

struct PhonemeInfoKey

Keys for the speech phoneme information.

Deprecated

struct StatusKey

Keys for the speech synthesizier status.

Deprecated

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

Deprecated

