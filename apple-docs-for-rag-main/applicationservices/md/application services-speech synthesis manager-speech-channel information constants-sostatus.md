

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soStatus 

Global Variable

# soStatus

macOS 10.0+

``` source
var soStatus: OSType { get }
```

## Discussion

Get a speech status information structure forthe speech channel. The `speechInfo` parameteris a pointer to a speech status information structure, describedin SpeechStatusInfo.

This selector works with the `GetSpeechInfo` function.

