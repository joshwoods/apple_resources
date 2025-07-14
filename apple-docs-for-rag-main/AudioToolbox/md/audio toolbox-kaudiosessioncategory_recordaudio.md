

- Audio Toolbox
-  kAudioSessionCategory_RecordAudio 

Global Variable

# kAudioSessionCategory_RecordAudio

For recording audio; this category silences playback audio. Recording continues with the screen locked.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionCategory_RecordAudio: Int { get }
```

## Discussion

This category is equivalent to the record category provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionCategory_AmbientSound: Int

For an app in which sound playback is nonprimary—that is, your app can be used successfully with the sound turned off.

Deprecated

var kAudioSessionCategory_SoloAmbientSound: Int

The default category, used unless you set a category with the AudioSessionSetProperty(_:_:_:) function.

var kAudioSessionCategory_MediaPlayback: Int

For playing recorded music or other sounds that are central to the successful use of your app.

var kAudioSessionCategory_PlayAndRecord: Int

Allows recording (input) and playback (output) of audio, such as for a VOIP (voice over IP) app.

var kAudioSessionCategory_AudioProcessing: Int

For using an audio hardware codec or signal processor while not playing or recording audio. Use this category, for example, when performing offline audio format conversion.

