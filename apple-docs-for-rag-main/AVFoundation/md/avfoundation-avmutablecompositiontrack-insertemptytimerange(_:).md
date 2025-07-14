

- AVFoundation
- AVMutableCompositionTrack
-  insertEmptyTimeRange(\_:) 

Instance Method

# insertEmptyTimeRange(\_:)

Adds or extends an empty time range within the track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func insertEmptyTimeRange(_ timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The empty time range to insert.

## See Also

### Managing Time Ranges

var segments: [AVCompositionTrackSegment]!

The track segments that a composition track contains.

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime) throws

Inserts a time range of media from a source track into a composition track.

func insertTimeRanges([NSValue], of: [AVAssetTrack], at: CMTime) throws

Inserts the time ranges of multiple source tracks into a track of a composition.

func removeTimeRange(CMTimeRange)

Removes a time range of media from a composition track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range of the track.

