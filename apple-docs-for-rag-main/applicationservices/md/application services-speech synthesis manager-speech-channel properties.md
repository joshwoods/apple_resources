

- Application Services
- Speech Synthesis Manager
-  Speech-Channel Properties 

API Collection

# Speech-Channel Properties

Properties used with CopySpeechProperty(_:_:_:) or SetSpeechProperty(_:_:_:) to get or set the characteristics of a speech channel.

## Topics

### Constants

let kSpeechStatusProperty: CFString

Get speech-status information for the speech channel.

let kSpeechErrorsProperty: CFString

Get speech-error information for the speech channel.

let kSpeechInputModeProperty: CFString

Get or set the speech channel’s current text-processing mode.

let kSpeechCharacterModeProperty: CFString

Get or set the speech channel’s current character-processing mode.

let kSpeechNumberModeProperty: CFString

Get or set the speech channel’s current number-processing mode.

let kSpeechRateProperty: CFString

Get or set a speech channel’s speech rate.

let kSpeechPitchBaseProperty: CFString

Get or set the speech channel’s baseline speech pitch.

let kSpeechPitchModProperty: CFString

Get or set a speech channel’s pitch modulation.

let kSpeechVolumeProperty: CFString

Get or set the speech volume for a speech channel.

let kSpeechSynthesizerInfoProperty: CFString

Get information about the speech synthesizer being used on the specified speech channel.

let kSpeechRecentSyncProperty: CFString

Get the message code for the most recently encountered synchronization command.

let kSpeechPhonemeSymbolsProperty: CFString

Get a list of phoneme symbols and example words defined for the speech channel’s synthesizer.

let kSpeechCurrentVoiceProperty: CFString

Set the current voice on the current speech channel to the specified voice.

let kSpeechCommandDelimiterProperty: CFString

Set the embedded speech command delimiter characters to be used for the speech channel.

let kSpeechResetProperty: CFString

Set a speech channel back to its default state.

let kSpeechOutputToFileURLProperty: CFString

Set the speech output destination to a file or to the computer’s speakers.

let kSpeechOutputToExtAudioFileProperty: CFString

Set the speech output destination to an extended audio file or to the computer’s speakers.

let kSpeechRefConProperty: CFString

Set a speech channel’s reference constant value.

let kSpeechTextDoneCallBack: CFString

Set the callback function to be called when the Speech Synthesis Manager has finished processing speech being generated on the speech channel.

let kSpeechSpeechDoneCallBack: CFString

Set the callback function to be called when the Speech Synthesis Manager has finished generating speech on the speech channel.

let kSpeechSyncCallBack: CFString

Set the callback function to be called when the Speech Synthesis Manager encounters a synchronization command within an embedded speech command in text being processed on the speech channel.

let kSpeechPhonemeCallBack: CFString

Set the callback function to be called every time the Speech Synthesis Manager is about to generate a phoneme on the speech channel.

let kSpeechErrorCFCallBack: CFString

Set the callback function to be called when an error is encountered during the processing of an embedded command.

let kSpeechWordCFCallBack: CFString

Set the callback function to be called every time the Speech Synthesis Manager is about to generate a word on the speech channel.

let kSpeechPhonemeOptionsProperty: CFString

Get or set the options for the generation of phonetic output.

let kSpeechOutputToAudioDeviceProperty: CFString

Set the speech output destination to an audio device file or to the computer’s speakers.

