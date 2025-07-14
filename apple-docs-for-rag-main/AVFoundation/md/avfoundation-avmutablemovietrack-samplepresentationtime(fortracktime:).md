

- AVFoundation
- AVMutableMovieTrack
-  samplePresentationTime(forTrackTime:) 

Instance Method

# samplePresentationTime(forTrackTime:)

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func samplePresentationTime(forTrackTime trackTime: CMTime) -> CMTime
```

## Parameters 

`trackTime`  

The track time for which to request the sample presentation time.

## Return Value

The sample presentation time corresponding to the specified time; otherwise invalid if the time is out of range.

## See Also

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

var timescale: CMTimeScale

The time scale for tracks that contain the `moov` atom.

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

var estimatedDataRate: Float

The estimated data rate, in bits per second, of the media that the track references.

