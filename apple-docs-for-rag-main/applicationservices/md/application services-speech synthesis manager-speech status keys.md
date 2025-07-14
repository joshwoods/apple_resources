

- Application Services
- Speech Synthesis Manager
-  Speech Status Keys 

API Collection

# Speech Status Keys

Keys used with the `kSpeechStatusProperty` property to specify the status of the speech channel.

## Topics

### Constants

let kSpeechStatusOutputBusy: CFString

Indicates whether the speech channel is currently producing speech.

let kSpeechStatusOutputPaused: CFString

Indicates whether speech output in the speech channel has been paused by a call to the PauseSpeechAt(_:_:) function.

let kSpeechStatusNumberOfCharactersLeft: CFString

The number of characters left in the input string of text.

let kSpeechStatusPhonemeCode: CFString

The opcode for the phoneme that the speech channel is currently processing.

