

- AVFoundation
- AVAssetWriterDelegate
-  assetWriter(\_:didOutputSegmentData:segmentType:segmentReport:) 

Instance Method

# assetWriter(\_:didOutputSegmentData:segmentType:segmentReport:)

Tells the delegate that the asset writer output segment data and a report.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
optional func assetWriter(
    _ writer: AVAssetWriter,
    didOutputSegmentData segmentData: Data,
    segmentType: AVAssetSegmentType,
    segmentReport: AVAssetSegmentReport?
)
```

## Parameters 

`writer`  

The asset writer that output segment data.

`segmentData`  

The data for the segment.

`segmentType`  

The type of segment data.

`segmentReport`  

A report for the segment data.

## Discussion

The asset writer stops normal file writing when you implement this method.

## See Also

### Responding to Segment Output

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType)

Tells the delegate that the asset writer output segment data.

class AVAssetSegmentReport

An object that provides information about segment data.

