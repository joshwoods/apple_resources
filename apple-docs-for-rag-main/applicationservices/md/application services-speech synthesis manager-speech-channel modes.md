

- Application Services
- Speech Synthesis Manager
-  Speech-Channel Modes 

# Speech-Channel Modes

The available text-processing and number-processing modes for a speech channel.

## Topics

### Constants

var modeText: OSType

Used with soInputMode to indicate that the speech channel is in text-processing mode.

var modePhonemes: OSType

Used with soInputMode to indicate that the speech channel is in phoneme-processing mode. When in phoneme-processing mode, a text buffer is interpreted to be a series of characters representing various phonemes and prosodic controls.

var modeNormal: OSType

When the speech channel is in text-processing mode, indicates that the synthesizer should process characters as expected and assemble digits into numbers. Use this value with soCharacterMode and soNumberMode.

var modeLiteral: OSType

When the speech channel is in text-processing mode, indicates that characters and digits are spoken literally (for example, “cat” is spoken as “C-A-T” and “12” is spoken as "one, two"). Use this value with soCharacterMode and soNumberMode.

var modeTune: OSType

