

- Audio Toolbox
-  kAudioSessionCategory_SoloAmbientSound 

Global Variable

# kAudioSessionCategory_SoloAmbientSound

The default category, used unless you set a category with the AudioSessionSetProperty(_:_:_:) function.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionCategory_SoloAmbientSound: Int { get }
```

## Discussion

When you use this category, audio from other apps is silenced. Your audio is silenced by screen locking and by the Silent switch (called the *Ring/Silent switch* on iPhone).

This category is equivalent to the soloAmbient category provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionCategory_AmbientSound: Int

For an app in which sound playback is nonprimary—that is, your app can be used successfully with the sound turned off.

Deprecated

var kAudioSessionCategory_MediaPlayback: Int

For playing recorded music or other sounds that are central to the successful use of your app.

var kAudioSessionCategory_RecordAudio: Int

For recording audio; this category silences playback audio. Recording continues with the screen locked.

var kAudioSessionCategory_PlayAndRecord: Int

Allows recording (input) and playback (output) of audio, such as for a VOIP (voice over IP) app.

var kAudioSessionCategory_AudioProcessing: Int

For using an audio hardware codec or signal processor while not playing or recording audio. Use this category, for example, when performing offline audio format conversion.

