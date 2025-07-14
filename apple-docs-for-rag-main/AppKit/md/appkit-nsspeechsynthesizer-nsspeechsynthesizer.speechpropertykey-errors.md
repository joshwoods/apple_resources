

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
-  errors 

Type Property

# errors

Get speech-error information for the synthesizer.

macOS 10.5+

``` source
static let errors: NSSpeechSynthesizer.SpeechPropertyKey
```

## Discussion

A dictionary object that contains speech-error information. See NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey for a description of the keys present in the dictionary.

This property lets you get information about various run-time errors that occur during speaking, such as the detection of badly formed embedded commands. Errors returned directly by the Speech Synthesis Manager are not reported here.

If your application implements the speechSynthesizer(_:didEncounterErrorAt:of:message:) delegate message, the delegate message can use this property to get error information.

This property is used with setObject(_:forProperty:).

## See Also

### Speech Property Keys

static let status: NSSpeechSynthesizer.SpeechPropertyKey

Get speech-status information for the synthesizer.

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

