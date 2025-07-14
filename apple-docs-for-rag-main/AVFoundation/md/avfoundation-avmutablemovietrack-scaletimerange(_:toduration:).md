

- AVFoundation
- AVMutableMovieTrack
-  scaleTimeRange(\_:toDuration:) 

Instance Method

# scaleTimeRange(\_:toDuration:)

Changes the duration of a time range in a track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func scaleTimeRange(
    _ timeRange: CMTimeRange,
    toDuration duration: CMTime
)
```

## Parameters 

`timeRange`  

The time range to change.

`duration`  

The new duration for the time range.

## See Also

### Managing Time Ranges

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime, copySampleData: Bool) throws

Inserts a portion of an asset track into the target movie.

func insertEmptyTimeRange(CMTimeRange)

Adds an empty time range to a track.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a track.

