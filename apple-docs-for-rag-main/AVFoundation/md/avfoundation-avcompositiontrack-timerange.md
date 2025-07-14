

- AVFoundation
- AVCompositionTrack
-  timeRange 

Instance Property

# timeRange

The time range of the track within the overall timeline of the asset.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var timeRange: CMTimeRange { get }
```

## Discussion

If the start of the time range is greater than zero, the track doesn’t initially have media data to present. This condition may occur when the media delays an audio track to align the start of audio with a specific video frame. You can test for this as the example below shows:

```
if track.timeRange.start > .zero {
    // Delayed start.
}
```

## See Also

### Accessing Temporal Information

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

var estimatedDataRate: Float

The estimated data rate, in bits per second, of the media that the track references.

func samplePresentationTime(forTrackTime: CMTime) -> CMTime

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

