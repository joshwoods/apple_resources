

- AVFoundation
- AVMutableMovie
-  scale(\_:toDuration:) 

Instance Method

# scale(\_:toDuration:)

Changes the duration of a time range in a movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func scale(
    _ timeRange: CMTimeRange,
    toDuration duration: CMTime
)
```

## Parameters 

`timeRange`  

The time range to be changed.

`duration`  

The new duration for the time range.

## See Also

### Managing Time Ranges

func insertEmptyTimeRange(CMTimeRange)

Adds an empty time range to a movie.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, copySampleData: Bool) throws

Inserts all of the tracks in a specified time range of an asset into a movie.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a movie.

