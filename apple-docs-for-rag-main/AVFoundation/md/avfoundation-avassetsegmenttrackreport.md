

- AVFoundation
-  AVAssetSegmentTrackReport 

Class

# AVAssetSegmentTrackReport

An object that provides information on a track in segment data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class AVAssetSegmentTrackReport
```

## Topics

### Inspecting a Report

var trackID: CMPersistentTrackID

A persistent unique identifier for a track.

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

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Inspecting a Report

var segmentType: AVAssetSegmentType

The type of segment data.

enum AVAssetSegmentType

Constants that define the type of a segment.

var trackReports: [AVAssetSegmentTrackReport]

The reports for the segment’s track data.

