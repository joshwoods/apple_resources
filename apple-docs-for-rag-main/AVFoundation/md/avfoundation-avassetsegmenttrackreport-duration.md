

- AVFoundation
- AVAssetSegmentTrackReport
-  duration 

Instance Property

# duration

The duration of a track.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var duration: CMTime { get }
```

## Discussion

The value is invalid if there’s no information available.

## See Also

### Inspecting a Report

var trackID: CMPersistentTrackID

A persistent unique identifier for a track.

var mediaType: AVMediaType

The type of media a track contains.

var earliestPresentationTimeStamp: CMTime

The earliest presentation timestamp (PTS) for this track.

var firstVideoSampleInformation: AVAssetSegmentReportSampleInformation?

Information about the first video sample in a track.

class AVAssetSegmentReportSampleInformation

An object that provides information about sample data in a track.

