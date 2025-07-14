

- AVFoundation
- AVMutableCompositionTrack
-  scaleTimeRange(\_:toDuration:) 

Instance Method

# scaleTimeRange(\_:toDuration:)

Changes the duration of a time range of the track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func scaleTimeRange(
    _ timeRange: CMTimeRange,
    toDuration duration: CMTime
)
```

## Parameters 

`timeRange`  

The time range to scale.

`duration`  

A new duration value.

## See Also

### Managing Time Ranges

var segments: [AVCompositionTrackSegment]!

The track segments that a composition track contains.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within the track.

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime) throws

Inserts a time range of media from a source track into a composition track.

func insertTimeRanges([NSValue], of: [AVAssetTrack], at: CMTime) throws

Inserts the time ranges of multiple source tracks into a track of a composition.

func removeTimeRange(CMTimeRange)

Removes a time range of media from a composition track.

