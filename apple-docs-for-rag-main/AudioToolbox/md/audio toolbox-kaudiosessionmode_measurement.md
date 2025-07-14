

- Audio Toolbox
-  kAudioSessionMode_Measurement 

Global Variable

# kAudioSessionMode_Measurement

Specify this mode if your app is performing measurement of incoming audio.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionMode_Measurement: Int { get }
```

## Discussion

When this mode is in use, the device does not perform automatic gain adjustment on incoming audio. For use with the kAudioSessionCategory_RecordAudio or kAudioSessionCategory_PlayAndRecord audio session categories. On devices with more than one built-in microphone, the primary microphone is used.

This mode is equivalent to the measurement mode provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionMode_Default: Int

The default mode; used unless you set a mode with the AudioSessionSetProperty(_:_:_:) function.

Deprecated

var kAudioSessionMode_VoiceChat: Int

Specify this mode if your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

var kAudioSessionMode_VideoRecording: Int

Specify this mode if your app is recording a movie.

var kAudioSessionMode_GameChat: Int

