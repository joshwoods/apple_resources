

- AVFoundation
- AVSampleBufferDisplayLayer
-  preventsAutomaticBackgroundingDuringVideoPlayback 

Instance Property

# preventsAutomaticBackgroundingDuringVideoPlayback

A Boolean value that indicates whether video playback prevents the system from automatically backgrounding an app.

visionOS 1.0+

``` source
var preventsAutomaticBackgroundingDuringVideoPlayback: Bool { get set }
```

## Discussion

The default value is true, which indicates the system doesn’t automatically background an app while playing video. The value of this property doesn’t prevent the user from backgrounding an app.

Note

When enqueuing sample buffers for playback at the user’s request, set the value to true, and when video playback isn’t the user’s primary focus, set it to false.

## See Also

### Preventing backgrounding

var preventsDisplaySleepDuringVideoPlayback: Bool

A Boolean value that indicates whether the layer prevents the system from sleeping during video playback.

