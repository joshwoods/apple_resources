

- AVFoundation
- AVAssetSegmentReportSampleInformation
-  presentationTimeStamp 

Instance Property

# presentationTimeStamp

The presentation timestamp (PTS) of a sample.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var presentationTimeStamp: CMTime { get }
```

## Discussion

This timestamp may be different from the earliestPresentationTimeStamp if the video’s author encodes it using frame reordering.

## See Also

### Inspecting the Information

var offset: Int

The offset of a sample in the segment.

var length: Int

The length of the sample data.

var isSyncSample: Bool

A Boolean value that indicates whether the sample is a key frame.

