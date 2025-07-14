

- Audio Toolbox
-  kAudioSessionMode_Default Deprecated

Global Variable

# kAudioSessionMode_Default

The default mode; used unless you set a mode with the AudioSessionSetProperty(_:_:_:) function.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionMode_Default: Int { get }
```

Deprecated

Deprecated in iOS 7.0.

## Discussion

When this mode is in use, audio session behavior matches that of iOS versions prior to iOS 5.0. You can use this mode with every audio session category. On devices with more than one built-in microphone, the primary microphone is used.

This mode is equivalent to the default mode provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionMode_VoiceChat: Int

Specify this mode if your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

var kAudioSessionMode_VideoRecording: Int

Specify this mode if your app is recording a movie.

var kAudioSessionMode_Measurement: Int

Specify this mode if your app is performing measurement of incoming audio.

var kAudioSessionMode_GameChat: Int

