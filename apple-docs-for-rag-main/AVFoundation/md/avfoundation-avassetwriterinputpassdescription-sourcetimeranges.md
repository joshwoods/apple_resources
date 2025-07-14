

- AVFoundation
- AVAssetWriterInputPassDescription
-  sourceTimeRanges 

Instance Property

# sourceTimeRanges

An array of time ranges.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var sourceTimeRanges: [NSValue] { get }
```

## Discussion

Each element in the array is an NSValue object that wraps a CMTimeRange structure that represents one source time range. The value of this property is suitable to pass to the reset(forReadingTimeRanges:) method of AVAssetReaderOutput.

