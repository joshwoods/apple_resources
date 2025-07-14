

- Core Media
-  CMTimeRangeEqual(\_:\_:) 

Function

# CMTimeRangeEqual(\_:\_:)

Returns a Boolean value that indicates whether two time ranges are equal.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeEqual(
    _ range1: CMTimeRange,
    _ range2: CMTimeRange
) -> Bool
```

## Parameters 

`range1`  

The first time range to compare.

`range2`  

The second time range to compare.

## Return Value

true if the two time ranges are equal; otherwise, false.

## See Also

### Comparing Time Ranges

func CMTimeRangeContainsTime(CMTimeRange, time: CMTime) -> Bool

Returns a Boolean value that indicates whether a time range contains a time.

func CMTimeRangeContainsTimeRange(CMTimeRange, otherRange: CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range contains another time range.

