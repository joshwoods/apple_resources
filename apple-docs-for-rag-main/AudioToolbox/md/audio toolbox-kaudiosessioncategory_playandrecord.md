

- Audio Toolbox
-  kAudioSessionCategory_PlayAndRecord 

Global Variable

# kAudioSessionCategory_PlayAndRecord

Allows recording (input) and playback (output) of audio, such as for a VOIP (voice over IP) app.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionCategory_PlayAndRecord: Int { get }
```

## Discussion

Your audio continues with the Silent switch set to silent and with the screen locked. (The switch is called the *Ring/Silent switch* on iPhone.)

This category is appropriate for simultaneous recording and playback, and also for apps that record and play back but not simultaneously. If you want to ensure that sounds such as Messages alerts do not play while your app is recording, use the kAudioSessionCategory_RecordAudio category instead.

This category normally prevents audio from other apps from mixing with your app’s audio. To allow mixing when using this category, use the kAudioSessionProperty_OverrideCategoryMixWithOthers property.

This category is equivalent to the playAndRecord category provided in the AVFoundation framework.

## See Also

### Constants

var kAudioSessionCategory_AmbientSound: Int

For an app in which sound playback is nonprimary—that is, your app can be used successfully with the sound turned off.

Deprecated

var kAudioSessionCategory_SoloAmbientSound: Int

The default category, used unless you set a category with the AudioSessionSetProperty(_:_:_:) function.

var kAudioSessionCategory_MediaPlayback: Int

For playing recorded music or other sounds that are central to the successful use of your app.

var kAudioSessionCategory_RecordAudio: Int

For recording audio; this category silences playback audio. Recording continues with the screen locked.

var kAudioSessionCategory_AudioProcessing: Int

For using an audio hardware codec or signal processor while not playing or recording audio. Use this category, for example, when performing offline audio format conversion.

