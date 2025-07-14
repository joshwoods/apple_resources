

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechOutputToAudioDeviceProperty 

Global Variable

# kSpeechOutputToAudioDeviceProperty

Set the speech output destination to an audio device file or to the computer’s speakers.

macOS 10.6+

``` source
let kSpeechOutputToAudioDeviceProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object that contains an AudioDeviceID. To play the speech output to an audio device, use the AudioDeviceID that represents the device; to generate sound through the computer’s speakers, use `0`.

This property works with the SetSpeechProperty(_:_:_:) function.

