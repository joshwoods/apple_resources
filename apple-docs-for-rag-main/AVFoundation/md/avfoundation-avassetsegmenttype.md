

- AVFoundation
-  AVAssetSegmentType 

Enumeration

# AVAssetSegmentType

Constants that define the type of a segment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum AVAssetSegmentType
```

## Topics

### Segment Types

case initialization

An initialization segment type.

case separable

A separable segment type.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Report

var segmentType: AVAssetSegmentType

The type of segment data.

var trackReports: [AVAssetSegmentTrackReport]

The reports for the segment’s track data.

class AVAssetSegmentTrackReport

An object that provides information on a track in segment data.

