

- AVFoundation
- AVPlayer
-  preventsAutomaticBackgroundingDuringVideoPlayback 

Instance Property

# preventsAutomaticBackgroundingDuringVideoPlayback

A Boolean value that indicates whether video playback prevents the system from automatically backgrounding the app.

visionOS 1.0+

``` source
nonisolated
var preventsAutomaticBackgroundingDuringVideoPlayback: Bool { get set }
```

## Discussion

The default value is true, which indicates the system doesn’t automatically background an app while it’s actively playing video. A user may still choose to background an app.

## See Also

### Preventing Sleep and Backgrounding

var preventsDisplaySleepDuringVideoPlayback: Bool

A Boolean value that indicates whether video playback prevents display and device sleep.

