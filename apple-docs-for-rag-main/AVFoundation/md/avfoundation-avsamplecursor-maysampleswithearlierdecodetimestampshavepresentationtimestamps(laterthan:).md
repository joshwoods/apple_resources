

- AVFoundation
- AVSampleCursor
-  maySamplesWithEarlierDecodeTimeStampsHavePresentationTimeStamps(laterThan:) 

Instance Method

# maySamplesWithEarlierDecodeTimeStampsHavePresentationTimeStamps(laterThan:)

Determines whether a sample earlier in decode order can have a presentation timestamp later than that of the specified sample cursor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func maySamplesWithEarlierDecodeTimeStampsHavePresentationTimeStamps(laterThan cursor: AVSampleCursor) -> Bool
```

## Parameters 

`cursor`  

An instance of `AVSampleCursor` with which to test the sample reordering boundary.

## Return Value

true if it’s possible for any sample earlier in decode order than the sample at the position of the receiver can have a presentation timestamp later than that of the specified sample cursor; otherwise, false.

## Discussion

Undefined results occur if this cursor and the passed in cursor reference different sequences of samples, such as when they’re created by different instances of AVAssetTrack.

## See Also

### Accessing Samples

func maySamplesWithLaterDecodeTimeStampsHavePresentationTimeStamps(earlierThan: AVSampleCursor) -> Bool

Determines whether a sample later in decode order can have a presentation timestamp earlier than that of the specified sample cursor.

var samplesRequiredForDecoderRefresh: Int

The number of samples prior to the current sample, in decode order, the decoder requires to achieve a coherent output at the current decode time.

