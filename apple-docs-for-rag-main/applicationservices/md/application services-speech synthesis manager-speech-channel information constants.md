

- Application Services
- Speech Synthesis Manager
-  Speech-Channel Information Constants 

# Speech-Channel Information Constants

Selectors that can be passed to the `GetSpeechInfo` or `SetSpeechInfo` functions.

## Overview

See the GetSpeechInfo and SetSpeechInfo functions.

## Topics

### Constants

var soStatus: OSType

var soErrors: OSType

var soInputMode: OSType

var soCharacterMode: OSType

var soNumberMode: OSType

var soRate: OSType

var soPitchBase: OSType

var soPitchMod: OSType

var soVolume: OSType

var soSynthType: OSType

var soRecentSync: OSType

var soPhonemeSymbols: OSType

var soCurrentVoice: OSType

var soCommandDelimiter: OSType

var soReset: OSType

var soCurrentA5: OSType

var soRefCon: OSType

var soTextDoneCallBack: OSType

var soSpeechDoneCallBack: OSType

var soSyncCallBack: OSType

var soErrorCallBack: OSType

var soPhonemeCallBack: OSType

var soWordCallBack: OSType

var soSynthExtension: OSType

var soSoundOutput: OSType

Get or set the speech channel’s current outputchannel.

var soOutputToFileWithCFURL: OSType

Pass a `CFURLRef` in the `speechInfo` parameter to write to this file, or `NULL` to generate sound.

var soOutputToExtAudioFile: OSType

Pass an ExtAudioFileRef in the `speechInfo` parameter to write to this file, or `NULL` to generate sound.

var soPhonemeOptions: OSType

Get or set options for the generation of phonetic output. See Phoneme Generation Options for a complete list of options.

var soOutputToAudioDevice: OSType

