

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  NSSpeechSynthesizer.SpeechPropertyKey.StatusKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Keys for the speech synthesizier status.

macOS 10.3–14.0Deprecated

``` source
struct StatusKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

Use these keys in the status dictionary.

## Topics

### Status Keys

static let numberOfCharactersLeft: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

The number of characters left in the input string of text.

static let outputBusy: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates whether the synthesizer is currently producing speech.

static let outputPaused: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates whether speech output in the synthesizer has been paused by sending the message pauseSpeaking(at:).

static let phonemeCode: NSSpeechSynthesizer.SpeechPropertyKey.StatusKey

Indicates that the synthesizer is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

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

struct SynthesizerInfoKey

Keys for the speech synthesizier information.

Deprecated

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

Deprecated

