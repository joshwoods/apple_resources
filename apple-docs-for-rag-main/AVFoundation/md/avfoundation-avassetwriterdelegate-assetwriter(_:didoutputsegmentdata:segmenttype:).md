

- AVFoundation
- AVAssetWriterDelegate
-  assetWriter(\_:didOutputSegmentData:segmentType:) 

Instance Method

# assetWriter(\_:didOutputSegmentData:segmentType:)

Tells the delegate that the asset writer output segment data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
optional func assetWriter(
    _ writer: AVAssetWriter,
    didOutputSegmentData segmentData: Data,
    segmentType: AVAssetSegmentType
)
```

## Parameters 

`writer`  

The asset writer that output segment data.

`segmentData`  

The data for the segment.

`segmentType`  

The type of segment data.

## See Also

### Responding to Segment Output

func assetWriter(AVAssetWriter, didOutputSegmentData: Data, segmentType: AVAssetSegmentType, segmentReport: AVAssetSegmentReport?)

Tells the delegate that the asset writer output segment data and a report.

class AVAssetSegmentReport

An object that provides information about segment data.

