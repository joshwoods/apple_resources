

- AVFoundation
- AVMutableCompositionTrack
-  insertTimeRange(\_:of:at:) 

Instance Method

# insertTimeRange(\_:of:at:)

Inserts a time range of media from a source track into a composition track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func insertTimeRange(
    _ timeRange: CMTimeRange,
    of track: AVAssetTrack,
    at startTime: CMTime
) throws
```

## Parameters 

`timeRange`  

The time range of media in the source track to add.

`track`  

The source asset track that contains the media to add.

`startTime`  

A start time within the composition track to insert the time range.

## Discussion

The time range you insert presents at its natural duration and rate. If necessary, you can scale it to a different duration by calling the scaleTimeRange(_:toDuration:) method.

## See Also

### Managing Time Ranges

var segments: [AVCompositionTrackSegment]!

The track segments that a composition track contains.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within the track.

func insertTimeRanges([NSValue], of: [AVAssetTrack], at: CMTime) throws

Inserts the time ranges of multiple source tracks into a track of a composition.

func removeTimeRange(CMTimeRange)

Removes a time range of media from a composition track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range of the track.

