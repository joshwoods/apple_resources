

- AVFoundation
- AVMutableMovieTrack
-  insertEmptyTimeRange(\_:) 

Instance Method

# insertEmptyTimeRange(\_:)

Adds an empty time range to a track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func insertEmptyTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

A time range to insert.

## Discussion

You can’t add empty time ranges to the end of a track.

## See Also

### Managing Time Ranges

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime, copySampleData: Bool) throws

Inserts a portion of an asset track into the target movie.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range in a track.

