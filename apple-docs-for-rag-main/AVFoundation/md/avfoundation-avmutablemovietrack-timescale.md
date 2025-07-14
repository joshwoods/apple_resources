

- AVFoundation
- AVMutableMovieTrack
-  timescale 

Instance Property

# timescale

The time scale for tracks that contain the `moov` atom.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var timescale: CMTimeScale { get set }
```

## Discussion

The default media time is `0`. Set this property on any new, empty tracks before any edits are performed on the track.

## See Also

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

var estimatedDataRate: Float

The estimated data rate, in bits per second, of the media that the track references.

func samplePresentationTime(forTrackTime: CMTime) -> CMTime

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

