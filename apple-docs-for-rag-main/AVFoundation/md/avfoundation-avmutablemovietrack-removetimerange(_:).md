

- AVFoundation
- AVMutableMovieTrack
-  removeTimeRange(\_:) 

Instance Method

# removeTimeRange(\_:)

Removes the specified time range from a track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func removeTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The time range to remove.

## See Also

### Managing Time Ranges

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime, copySampleData: Bool) throws

Inserts a portion of an asset track into the target movie.

func insertEmptyTimeRange(CMTimeRange)

Adds an empty time range to a track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range in a track.

