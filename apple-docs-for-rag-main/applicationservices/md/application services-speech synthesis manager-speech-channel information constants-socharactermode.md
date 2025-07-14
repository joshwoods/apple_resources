

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soCharacterMode 

Global Variable

# soCharacterMode

macOS 10.0+

``` source
var soCharacterMode: OSType { get }
```

## Discussion

Get or set the speech channel’s character-processingmode. Two constants are currently defined for the processing mode, modeNormal and modeLiteral. Whenthe character-processing mode is `modeNormal`,input characters are spoken as you would expect to hear them. Whenthe mode is `modeLiteral`, eachcharacter is spoken literally, so that the word “cat” wouldbe spoken “C–A–T”. The `speechInfo` parameterpoints to a variable of type `OSType`, whichis the character-processing mode.

This selector works with the `GetSpeechInfo` and `SetSpeechInfo` functions.

