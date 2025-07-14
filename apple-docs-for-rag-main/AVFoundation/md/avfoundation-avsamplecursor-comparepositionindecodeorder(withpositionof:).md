

- AVFoundation
- AVSampleCursor
-  comparePositionInDecodeOrder(withPositionOf:) 

Instance Method

# comparePositionInDecodeOrder(withPositionOf:)

Compares the relative positions of two sample cursors and returns their relative positions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func comparePositionInDecodeOrder(withPositionOf cursor: AVSampleCursor) -> ComparisonResult
```

## Parameters 

`cursor`  

An instance of `AVSampleCursor` with which to compare positions.

## Return Value

Returns a comparison result that indicates of this cursor points at a sample before, the same as, or after the sample pointed to by the specified cursor.

## Discussion

Undefined results occur if this cursor and the passed in cursor reference different sequences of samples, such as when they’re created by different instances of AVAssetTrack.

