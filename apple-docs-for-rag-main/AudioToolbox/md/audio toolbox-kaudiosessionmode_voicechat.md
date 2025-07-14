

- Audio Toolbox
-  kAudioSessionMode_VoiceChat 

Global Variable

# kAudioSessionMode_VoiceChat

Specify this mode if your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionMode_VoiceChat: Int { get }
```

## Discussion

When this mode is in use, the device’s tonal equalization is optimized for voice. For use with the kAudioSessionCategory_PlayAndRecord audio session category. On devices with more than one built-in microphone, the primary microphone is used.

Using this mode has the side effect of setting the kAudioSessionProperty_OverrideCategoryEnableBluetoothInput category override to `TRUE`.

This mode is equivalent to the voiceChat mode provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionMode_Default: Int

The default mode; used unless you set a mode with the AudioSessionSetProperty(_:_:_:) function.

Deprecated

var kAudioSessionMode_VideoRecording: Int

Specify this mode if your app is recording a movie.

var kAudioSessionMode_Measurement: Int

Specify this mode if your app is performing measurement of incoming audio.

var kAudioSessionMode_GameChat: Int

