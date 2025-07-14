

- AppKit
-  NSSpeechSynthesizer Deprecated

Class

# NSSpeechSynthesizer

The Cocoa interface to speech synthesis in macOS.

macOS 10.3–14.0Deprecated

``` source
class NSSpeechSynthesizer
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Overview

Speech synthesis, also called text-to-speech (TTS), parses text and converts it into audible speech. It offers a concurrent feedback mode that can be used in concert with or in place of traditional visual and aural notifications. For example, your application can use a speech synthesizer object to “pronounce” the text of important alert dialogs. Synthesized speech has several advantages. It can provide urgent information to users without forcing them to shift attention from their current task. And because speech doesn’t rely on visual elements for meaning, it is a crucial technology for users with vision or attention disabilities.

In addition, synthesized speech can help save system resources. Because sound samples can take up large amounts of room on disk, using text in place of sampled sound is extremely efficient, and so a multimedia application might use an NSSpeechSynthesizer object to provide a narration of a QuickTime movie instead of including sampled-sound data on a movie track.

When you create an NSSpeechSynthesizer instance using the default initializer (`init`), the class uses the **default voice** selected in System Preferences \> Speech. Alternatively, you can select a specific voice for an NSSpeechSynthesizer instance by initializing it with init(voice:). To begin synthesis, send either startSpeaking(_:) or startSpeaking(_:to:) to the instance. The former generates speech through the system’s default sound output device; the latter saves the generated speech to a file. If you wish to be notified when the current speech concludes, set the delegate property and implement the delegate method speechSynthesizer(_:didFinishSpeaking:).

Speech synthesis is just one of the macOS speech technologies. The speech recognizer technology allows applications to “listen to” text spoken in U.S. English; the NSSpeechRecognizer class is the Cocoa interface to this technology. Both technologies provide benefits for all users, and are particularly useful to those users who have difficulties seeing the screen or using the mouse and keyboard.

### Speech Feedback Window

The speech feedback window (Figure 1) displays the text recognized from the user’s speech and the text from which an `NSSpeechSynthesizer` object synthesizes speech. Using the feedback window makes spoken exchange more natural and helps the user understand the synthesized speech.

For example, your application may use an NSSpeechRecognizer object to listen for the command “Play some music.” When it recognizes this command, your application might then respond by speaking “Which artist?” using a speech synthesizer.

When `UsesFeedbackWindow` is true, the speech synthesizer uses the feedback window if its visible, which the user specifies in System Preferences \> Speech.

## Topics

### Creating a Speech Synthesizer

init?(voice: NSSpeechSynthesizer.VoiceName?)

Initializes the receiver with a voice.

### Customizing the Speech Synthesizer Behavior

var delegate: (any NSSpeechSynthesizerDelegate)?

The synthesizer’s delegate.

protocol NSSpeechSynthesizerDelegate

A set of optional methods implemented by delegates of NSSpeechSynthesizer objects.

### Configuring Speech Synthesizers

var usesFeedbackWindow: Bool

Indicates whether the receiver uses the speech feedback window.

func voice() -> NSSpeechSynthesizer.VoiceName?

Returns the identifier of the receiver’s current voice.

func setVoice(NSSpeechSynthesizer.VoiceName?) -> Bool

Sets the receiver’s current voice.

var rate: Float

The synthesizer’s speaking rate (words per minute).

var volume: Float

The synthesizer’s speaking volume.

### Configuring Speech Attributes

func addSpeechDictionary([NSSpeechSynthesizer.DictionaryKey : Any])

Registers the given speech dictionary with the receiver.

struct DictionaryKey

These constants identify key-value pairs used to add vocabulary to the dictionary using addSpeechDictionary(_:).

func object(forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws -> Any

Provides the value of a receiver’s property.

func setObject(Any?, forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws

Specifies the value of a receiver’s property.

struct SpeechPropertyKey

These constants are used with setObject(_:forProperty:) and object(forProperty:) to get or set the characteristics of a synthesizer.

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

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

### Getting Speech Synthesizer Information

class var availableVoices: [NSSpeechSynthesizer.VoiceName]

Provides the identifiers of the voices available on the system.

class func attributes(forVoice: NSSpeechSynthesizer.VoiceName) -> [NSSpeechSynthesizer.VoiceAttributeKey : Any]

Provides the attribute dictionary of a voice.

class var defaultVoice: NSSpeechSynthesizer.VoiceName

Provides the identifier of the default voice.

struct VoiceName

struct VoiceAttributeKey

The following constants are keys for the dictionary returned by attributes(forVoice:).

### Getting Speech State

class var isAnyApplicationSpeaking: Bool

A Boolean value indicating whether any application is currently speaking through the sound output device.

### Synthesizing Speech

var isSpeaking: Bool

Indicates whether the receiver is currently generating synthesized speech.

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

func startSpeaking(String, to: URL) -> Bool

Begins synthesizing text into a sound (AIFF) file.

func pauseSpeaking(at: NSSpeechSynthesizer.Boundary)

Pauses synthesis in progress at a given boundary.

func continueSpeaking()

Resumes synthesis.

func stopSpeaking()

Stops synthesis in progress.

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

### Getting Phonemes

func phonemes(from: String) -> String

Provides the phoneme symbols generated by the given text.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Speech

class NSSpeechRecognizer

The Cocoa interface to speech recognition in macOS.

