

- Audio Toolbox
- Audio Session Support
-  Audio Session Categories 

API Collection

# Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

## Overview

Each app running in iOS has a single audio session, which in turn has a single category. You can change your audio session’s category while your app is running.

You can refine the configuration provided by the kAudioSessionCategory_RecordAudio and kAudioSessionCategory_PlayAndRecord categories by using an audio session mode, as described in Audio Session Modes.

Use the kAudioSessionCategory_AmbientSound category when you want your sounds to mix with other audio (such as from the iPod app). Use one of the other playback categories when you want audio from other apps to be silenced when your session is active. However, you can enable mixing for the kAudioSessionCategory_MediaPlayback and kAudioSessionCategory_PlayAndRecord categories by using the kAudioSessionProperty_OverrideCategoryMixWithOthers property. For more information on audio session categories, see Audio Session Programming Guide.

## Topics

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

var kAudioSessionCategory_PlayAndRecord: Int

Allows recording (input) and playback (output) of audio, such as for a VOIP (voice over IP) app.

var kAudioSessionCategory_AudioProcessing: Int

For using an audio hardware codec or signal processor while not playing or recording audio. Use this category, for example, when performing offline audio format conversion.

## See Also

### Audio Session Support

Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

