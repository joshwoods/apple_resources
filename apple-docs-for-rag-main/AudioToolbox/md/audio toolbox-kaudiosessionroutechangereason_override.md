

- Audio Toolbox
-  kAudioSessionRouteChangeReason_Override 

Global Variable

# kAudioSessionRouteChangeReason_Override

The audio route has been overridden.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionRouteChangeReason_Override: Int { get }
```

## Discussion

For example, while using the kAudioSessionCategory_PlayAndRecord category, output audio has been redirected to the speaker using the kAudioSessionProperty_OverrideAudioRoute property.

## See Also

### Constants

var kAudioSessionRouteChangeReason_Unknown: Int

The audio route changed but the reason is not known.

Deprecated

var kAudioSessionRouteChangeReason_NewDeviceAvailable: Int

A new audio hardware device became available; for example, a headset was plugged in.

var kAudioSessionRouteChangeReason_OldDeviceUnavailable: Int

The previously-used audio hardware device is now unavailable; for example, a headset was unplugged.

var kAudioSessionRouteChangeReason_CategoryChange: Int

The audio session category has changed.

var kAudioSessionRouteChangeReason_WakeFromSleep: Int

The device woke from sleep.

var kAudioSessionRouteChangeReason_NoSuitableRouteForCategory: Int

There is no audio hardware route for the audio session category.

var kAudioSessionRouteChangeReason_RouteConfigurationChange: Int

