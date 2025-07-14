

- Audio Toolbox
- Audio Session Support
-  Audio Session Modes 

API Collection

# Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

## Overview

Each app running in iOS has a single audio session, which in turn has a single mode. A mode refines the device’s audio configuration according to the purpose of the mode. You can change your audio session’s mode only when your audio session is inactive, and only if your audio session category is configured to disallow mixing with other apps.

Note

Misusing a mode by setting it for an inappropriate audio session category—such as setting the kAudioSessionMode_VoiceChat mode for the kAudioSessionCategory_AudioProcessing category—results in the behavior provided by the kAudioSessionMode_Default mode.

## Topics

### Constants

var kAudioSessionMode_Default: Int

The default mode; used unless you set a mode with the AudioSessionSetProperty(_:_:_:) function.

Deprecated

var kAudioSessionMode_VoiceChat: Int

Specify this mode if your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

var kAudioSessionMode_VideoRecording: Int

Specify this mode if your app is recording a movie.

var kAudioSessionMode_Measurement: Int

Specify this mode if your app is performing measurement of incoming audio.

var kAudioSessionMode_GameChat: Int

## See Also

### Audio Session Support

Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

