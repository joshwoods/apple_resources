

- Audio Toolbox
- Audio Session Support
-  Audio Session Activation Flags 

API Collection

# Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

## Topics

### Constants

var kAudioSessionSetActiveFlag_NotifyOthersOnDeactivation: Int

Indicates that when your audio session deactivates, other audio sessions that had been interrupted by your session can return to their active state.

Deprecated

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

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

