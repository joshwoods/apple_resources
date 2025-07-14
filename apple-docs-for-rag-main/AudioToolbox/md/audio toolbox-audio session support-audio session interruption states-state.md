

- Audio Toolbox
- Audio Session Support
-  Audio Session Interruption States 

API Collection

# Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

## Topics

### Constants

var kAudioSessionBeginInterruption: Int

Your app’s audio session has just been interrupted, such as by a phone call.

Deprecated

var kAudioSessionEndInterruption: Int

The interruption to your app’s audio session has just ended. In the case where a user confirms the interruption, such as answering a phone call, your app will not receive this constant.

## See Also

### Audio Session Support

Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

