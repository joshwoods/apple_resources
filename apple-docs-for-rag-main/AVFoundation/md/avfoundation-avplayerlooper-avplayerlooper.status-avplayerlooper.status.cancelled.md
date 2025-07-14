

- AVFoundation
- AVPlayerLooper
- AVPlayerLooper.Status
-  AVPlayerLooper.Status.cancelled 

Case

# AVPlayerLooper.Status.cancelled

The app canceled looping on the player.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case cancelled
```

## Discussion

The system sets this status after you call the disableLooping() method.

## See Also

### Status Values

case unknown

The status isn’t known.

case ready

The looper is ready to perform looping playback.

case failed

The looper isn’t able to perform looping playback due to an error.

