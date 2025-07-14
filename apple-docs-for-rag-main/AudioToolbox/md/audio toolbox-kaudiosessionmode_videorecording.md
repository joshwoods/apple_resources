

- Audio Toolbox
-  kAudioSessionMode_VideoRecording 

Global Variable

# kAudioSessionMode_VideoRecording

Specify this mode if your app is recording a movie.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionMode_VideoRecording: Int { get }
```

## Discussion

For use with the kAudioSessionCategory_RecordAudio audio session category. Also works with the kAudioSessionCategory_PlayAndRecord category. On devices with more than one built-in microphone, the microphone closest to the video camera is used.

Using this mode may result in the system providing appropriate audio signal processing.

This mode is equivalent to the videoRecording mode provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionMode_Default: Int

The default mode; used unless you set a mode with the AudioSessionSetProperty(_:_:_:) function.

Deprecated

var kAudioSessionMode_VoiceChat: Int

Specify this mode if your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

var kAudioSessionMode_Measurement: Int

Specify this mode if your app is performing measurement of incoming audio.

var kAudioSessionMode_GameChat: Int

