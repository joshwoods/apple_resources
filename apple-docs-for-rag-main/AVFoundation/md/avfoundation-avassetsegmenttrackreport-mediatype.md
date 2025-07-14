

- AVFoundation
- AVAssetSegmentTrackReport
-  mediaType 

Instance Property

# mediaType

The type of media a track contains.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var mediaType: AVMediaType { get }
```

## See Also

### Inspecting a Report

var trackID: CMPersistentTrackID

A persistent unique identifier for a track.

var duration: CMTime

The duration of a track.

var earliestPresentationTimeStamp: CMTime

The earliest presentation timestamp (PTS) for this track.

var firstVideoSampleInformation: AVAssetSegmentReportSampleInformation?

Information about the first video sample in a track.

class AVAssetSegmentReportSampleInformation

An object that provides information about sample data in a track.

