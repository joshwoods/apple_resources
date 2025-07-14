

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  characterMode 

Type Property

# characterMode

Get or set the synthesizer’s current text-processing mode.

macOS 10.5+

``` source
static let characterMode: NSSpeechSynthesizer.SpeechPropertyKey
```

## Discussion

An NSString object that specifies whether the channel is currently in text input mode or phoneme input mode.The supported values are listed in NSSpeechSynthesizer.SpeechPropertyKey.Mode.

When the character-processing mode is normal, input characters are spoken as you would expect to hear them. When the mode is literal, each character is spoken literally, so that the word “cat” is spoken “`C–A–T`”.

This property is used with setObject(_:forProperty:) and object(forProperty:).

## See Also

### Speech Property Keys

static let status: NSSpeechSynthesizer.SpeechPropertyKey

Get speech-status information for the synthesizer.

static let errors: NSSpeechSynthesizer.SpeechPropertyKey

Get speech-error information for the synthesizer.

static let inputMode: NSSpeechSynthesizer.SpeechPropertyKey

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

