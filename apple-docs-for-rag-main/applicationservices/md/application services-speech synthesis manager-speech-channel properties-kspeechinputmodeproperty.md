

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechInputModeProperty 

Global Variable

# kSpeechInputModeProperty

Get or set the speech channel’s current text-processing mode.

macOS 10.5+

``` source
let kSpeechInputModeProperty: CFString
```

## Discussion

The value associated with this property is a `CFString` object that specifies whether the channel is currently in text input mode or phoneme input mode. The constants `kSpeechModeText` and `kSpeechModePhoneme` (defined in Speech-Channel Modes for Core Foundation-based Functions) are the possible values of this string.

When in phoneme-processing mode, a text string is interpreted to be a series of characters representing various phonemes and prosodic controls. Some synthesizers might support additional input-processing modes and define constants for these modes.

When in text-processing mode, you can also specify how characters and numbers should be processed using the kSpeechCharacterModeProperty and kSpeechNumberModeProperty.

This property works with the CopySpeechProperty(_:_:_:) and SetSpeechProperty(_:_:_:) functions.

