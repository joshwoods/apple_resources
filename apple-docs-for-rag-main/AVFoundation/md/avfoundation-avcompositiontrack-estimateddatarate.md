

- AVFoundation
- AVCompositionTrack
-  estimatedDataRate 

Instance Property

# estimatedDataRate

The estimated data rate, in bits per second, of the media that the track references.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var estimatedDataRate: Float { get }
```

## See Also

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

func samplePresentationTime(forTrackTime: CMTime) -> CMTime

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

