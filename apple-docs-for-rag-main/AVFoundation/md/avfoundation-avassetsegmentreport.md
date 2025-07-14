

- AVFoundation
-  AVAssetSegmentReport 

Class

# AVAssetSegmentReport

An object that provides information about segment data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class AVAssetSegmentReport
```

## Overview

You receive a segment report through the assetWriter(_:didOutputSegmentData:segmentType:segmentReport:) delegate method.

## Topics

### Inspecting a Report

var segmentType: AVAssetSegmentType

The type of segment data.

enum AVAssetSegmentType

Constants that define the type of a segment.

var trackReports: [AVAssetSegmentTrackReport]

The reports for the segment’s track data.

class AVAssetSegmentTrackReport

An object that provides information on a track in segment data.

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

### Responding to Segment Output

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType)

Tells the delegate that the asset writer output segment data.

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType, segmentReport: AVAssetSegmentReport?)

Tells the delegate that the asset writer output segment data and a report.

