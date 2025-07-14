

- Audio Toolbox
-  kAudioSessionRouteChangeReason_NoSuitableRouteForCategory 

Global Variable

# kAudioSessionRouteChangeReason_NoSuitableRouteForCategory

There is no audio hardware route for the audio session category.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionRouteChangeReason_NoSuitableRouteForCategory: Int { get }
```

## Discussion

For example, the kAudioSessionCategory_RecordAudio is set but there is no audio input device.

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

var kAudioSessionRouteChangeReason_Override: Int

The audio route has been overridden.

var kAudioSessionRouteChangeReason_WakeFromSleep: Int

The device woke from sleep.

var kAudioSessionRouteChangeReason_RouteConfigurationChange: Int

