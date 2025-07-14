

- AVFoundation
-  AVAssetSegmentReportSampleInformation 

Class

# AVAssetSegmentReportSampleInformation

An object that provides information about sample data in a track.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class AVAssetSegmentReportSampleInformation
```

## Topics

### Inspecting the Information

var presentationTimeStamp: CMTime

The presentation timestamp (PTS) of a sample.

var offset: Int

The offset of a sample in the segment.

var length: Int

The length of the sample data.

var isSyncSample: Bool

A Boolean value that indicates whether the sample is a key frame.

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

