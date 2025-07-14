

- AppKit
- NSSpeechSynthesizer
-  NSSpeechSynthesizer.SpeechPropertyKey Deprecated

Structure

# NSSpeechSynthesizer.SpeechPropertyKey

These constants are used with setObject(_:forProperty:) and object(forProperty:) to get or set the characteristics of a synthesizer.

macOS 10.3–14.0Deprecated

``` source
struct SpeechPropertyKey
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Topics

### Speech Property Keys

static let status: NSSpeechSynthesizer.SpeechPropertyKey

Get speech-status information for the synthesizer.

static let errors: NSSpeechSynthesizer.SpeechPropertyKey

Get speech-error information for the synthesizer.

static let inputMode: NSSpeechSynthesizer.SpeechPropertyKey

Get or set the synthesizer’s current text-processing mode.

static let characterMode: NSSpeechSynthesizer.SpeechPropertyKey

Get or set the synthesizer’s current text-processing mode.

static let numberMode: NSSpeechSynthesizer.SpeechPropertyKey

Get or set the synthesizer’s current number-processing mode.

static let rate: NSSpeechSynthesizer.SpeechPropertyKey

Get or set a synthesizer’s speech rate.

static let pitchBase: NSSpeechSynthesizer.SpeechPropertyKey

Get or set a synthesizer’s baseline speech pitch.

static let pitchMod: NSSpeechSynthesizer.SpeechPropertyKey

Get or set a synthesizer’s pitch modulation.

static let volume: NSSpeechSynthesizer.SpeechPropertyKey

Get or set the speech volume for a synthesizer.

static let synthesizerInfo: NSSpeechSynthesizer.SpeechPropertyKey

Get information about the speech synthesizer being used on the specified synthesizer.

static let recentSync: NSSpeechSynthesizer.SpeechPropertyKey

Get the message code for the most recently encountered synchronization command.

static let phonemeSymbols: NSSpeechSynthesizer.SpeechPropertyKey

Get a list of phoneme symbols and example words defined for the synthesizer.

static let currentVoice: NSSpeechSynthesizer.SpeechPropertyKey

Set the current voice on the synthesizer to the specified voice.

static let commandDelimiter: NSSpeechSynthesizer.SpeechPropertyKey

Set the embedded speech command delimiter characters to be used for the synthesizer.

static let reset: NSSpeechSynthesizer.SpeechPropertyKey

Set a synthesizer back to its default state.

static let outputToFileURL: NSSpeechSynthesizer.SpeechPropertyKey

Set the speech output destination to a file or to the computer’s speakers.

### Type Aliases

struct CommandDelimiterKey

Keys for the command delimiters.

struct ErrorKey

Keys that identify errors that may occur during speech synthesis.

struct Mode

Keys for the speaking mode.

struct PhonemeInfoKey

Keys for the speech phoneme information.

struct StatusKey

Keys for the speech synthesizier status.

struct SynthesizerInfoKey

Keys for the speech synthesizier information.

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

