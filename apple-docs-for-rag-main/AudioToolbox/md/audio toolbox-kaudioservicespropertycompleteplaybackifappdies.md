

- Audio Toolbox
-  kAudioServicesPropertyCompletePlaybackIfAppDies 

Global Variable

# kAudioServicesPropertyCompletePlaybackIfAppDies

A `UInt32` value, where `1` means that the audio file specified by a system sound passed in the `inSpecifier` parameter should finish playing even if the client application terminates. This could happen, for example, if the user quits or the application terminates unexpectedly while the sound is playing. The default is `0`. That is, you must explicitly set this property’s value to `1` if you want the sound to complete playing even if the application terminates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioServicesPropertyCompletePlaybackIfAppDies: AudioServicesPropertyID { get }
```

## See Also

### Constants

var kAudioServicesPropertyIsUISound: AudioServicesPropertyID

A `UInt32` value, where `1` means that, for the audio file specified by a system sound passed in the `inSpecifier` parameter, the System Sound server respects the user setting in the Sound Effects preference and is silent when the user turns off sound effects.

