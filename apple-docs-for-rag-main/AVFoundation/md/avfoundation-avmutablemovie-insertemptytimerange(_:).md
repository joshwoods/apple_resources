

- AVFoundation
- AVMutableMovie
-  insertEmptyTimeRange(\_:) 

Instance Method

# insertEmptyTimeRange(\_:)

Adds an empty time range to a movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func insertEmptyTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The time range to be made empty.

## Discussion

You can’t add empty time ranges to the end of a movie.

## See Also

### Managing Time Ranges

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, copySampleData: Bool) throws

Inserts all of the tracks in a specified time range of an asset into a movie.

func scale(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range in a movie.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a movie.

