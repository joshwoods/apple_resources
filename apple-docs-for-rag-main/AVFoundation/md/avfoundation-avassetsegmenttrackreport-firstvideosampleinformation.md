

- AVFoundation
- AVAssetSegmentTrackReport
-  firstVideoSampleInformation 

Instance Property

# firstVideoSampleInformation

Information about the first video sample in a track.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var firstVideoSampleInformation: AVAssetSegmentReportSampleInformation? { get }
```

## Discussion

The value is `nil` if this track isn’t a video track, or if sample information isn’t available.

## See Also

### Inspecting a Report

var trackID: CMPersistentTrackID

A persistent unique identifier for a track.

var mediaType: AVMediaType

The type of media a track contains.

var duration: CMTime

The duration of a track.

var earliestPresentationTimeStamp: CMTime

The earliest presentation timestamp (PTS) for this track.

class AVAssetSegmentReportSampleInformation

An object that provides information about sample data in a track.

