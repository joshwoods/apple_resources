

- AVFoundation
- AVAssetSegmentTrackReport
-  trackID 

Instance Property

# trackID

A persistent unique identifier for a track.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var trackID: CMPersistentTrackID { get }
```

## See Also

### Inspecting a Report

var mediaType: AVMediaType

The type of media a track contains.

var duration: CMTime

The duration of a track.

var earliestPresentationTimeStamp: CMTime

The earliest presentation timestamp (PTS) for this track.

var firstVideoSampleInformation: AVAssetSegmentReportSampleInformation?

Information about the first video sample in a track.

class AVAssetSegmentReportSampleInformation

An object that provides information about sample data in a track.

