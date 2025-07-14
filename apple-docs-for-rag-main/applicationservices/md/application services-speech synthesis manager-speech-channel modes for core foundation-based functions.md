

- Application Services
- Speech Synthesis Manager
-  Speech-Channel Modes for Core Foundation-based Functions 

API Collection

# Speech-Channel Modes for Core Foundation-based Functions

The available text-processing and number-processing modes for a speech channel.

## Topics

### Constants

let kSpeechModeText: CFString

Used with kSpeechInputModeProperty to indicate that the speech channel is in text-processing mode.

let kSpeechModePhoneme: CFString

Used with kSpeechInputModeProperty to indicate that the speech channel is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

let kSpeechModeNormal: CFString

When the speech channel is in text-processing mode, indicates that the synthesizer should process characters as expected and assemble digits into numbers. Use this value with kSpeechCharacterModeProperty and kSpeechNumberModeProperty.

let kSpeechModeLiteral: CFString

When the speech channel is in text-processing mode, indicates that characters and digits are spoken literally (for example, “cat” is spoken as “C-A-T” and “12” is spoken as "one, two"). Use this value with kSpeechCharacterModeProperty and kSpeechNumberModeProperty.

