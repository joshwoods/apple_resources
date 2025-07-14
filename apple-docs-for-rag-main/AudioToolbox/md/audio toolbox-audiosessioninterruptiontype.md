

- Audio Toolbox
-  AudioSessionInterruptionType 

Type Alias

# AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
typealias AudioSessionInterruptionType = UInt32
```

## Topics

### Constants

var kAudioSessionInterruptionType_ShouldResume: Int

Indicates that the interruption that has just ended was one for which it is appropriate to immediately resume playback; for example, an incoming phone call was rejected by the user.

Deprecated

var kAudioSessionInterruptionType_ShouldNotResume: Int

Indicates that the interruption that has just ended was one for which it is not appropriate to resume playback; for example, your app had been interrupted by iPod playback.

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

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

