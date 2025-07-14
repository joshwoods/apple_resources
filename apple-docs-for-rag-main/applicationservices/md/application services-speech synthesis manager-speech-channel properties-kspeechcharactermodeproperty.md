

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechCharacterModeProperty 

Global Variable

# kSpeechCharacterModeProperty

Get or set the speech channel’s current character-processing mode.

macOS 10.5+

``` source
let kSpeechCharacterModeProperty: CFString
```

## Discussion

The value associated with this property is a `CFString` object that specifies whether the speech channel is currently in normal or literal character-processing mode. The constants `kSpeechModeNormal` and `kSpeechModeLiteral` (defined in Speech-Channel Modes for Core Foundation-based Functions) are the possible values of this string.

When the character-processing mode is `kSpeechModeNormal`, input characters are spoken as you would expect to hear them. When the mode is `kSpeechModeLiteral`, each character is spoken literally, so that the word “cat” is spoken “C–A–T”.

This property works with the CopySpeechProperty(_:_:_:) and SetSpeechProperty(_:_:_:) functions.

