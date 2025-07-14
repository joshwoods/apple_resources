

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soOutputToAudioDevice 

Global Variable

# soOutputToAudioDevice

macOS 10.6+

``` source
var soOutputToAudioDevice: OSType { get }
```

## Discussion

Pass a pointer to an AudioDeviceID in the `speechInfo` parameter to play to this file, or `0` to play through the default audio output device.

This selector works with the `SetSpeechInfo` function.

