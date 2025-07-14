

- Core Media
-  CMTimeRangeContainsTimeRange(\_:otherRange:) 

Function

# CMTimeRangeContainsTimeRange(\_:otherRange:)

Returns a Boolean value that indicates whether a time range contains another time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeContainsTimeRange(
    _ range: CMTimeRange,
    otherRange: CMTimeRange
) -> Bool
```

## Parameters 

`range`  

The first time range to compare.

`otherRange`  

The second time range to test for inclusion.

## Return Value

true if `range1` contains `range2`; otherwise, false.

## See Also

### Comparing Time Ranges

func CMTimeRangeEqual(CMTimeRange, CMTimeRange) -> Bool

Returns a Boolean value that indicates whether two time ranges are equal.

func CMTimeRangeContainsTime(CMTimeRange, time: CMTime) -> Bool

Returns a Boolean value that indicates whether a time range contains a time.

