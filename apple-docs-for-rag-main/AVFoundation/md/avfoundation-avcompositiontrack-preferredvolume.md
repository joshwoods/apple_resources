

- AVFoundation
- AVCompositionTrack
-  preferredVolume 

Instance Property

# preferredVolume

The track’s volume preference for playing its audible media.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var preferredVolume: Float { get }
```

## Discussion

The preferred volume for an audio track is typically, but not always, `1.0`. For non-audible tracks, the value is `0.0`.

## See Also

### Accessing Audible Characteristics

var hasAudioSampleDependencies: Bool

A Boolean value that indicates whether the track has sample dependencies.

