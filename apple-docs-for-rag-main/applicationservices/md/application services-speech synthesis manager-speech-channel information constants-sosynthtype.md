

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soSynthType 

Global Variable

# soSynthType

macOS 10.0+

``` source
var soSynthType: OSType { get }
```

## Discussion

Get a speech version information structurefor the speech synthesizer being used on the specified speech channel.The `speechInfo` parameteris a pointer to a speech version information structure, describedin SpeechVersionInfo.

This selector works with the `GetSpeechInfo` function.

