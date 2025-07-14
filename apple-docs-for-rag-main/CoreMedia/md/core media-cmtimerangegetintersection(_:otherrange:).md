

- Core Media
-  CMTimeRangeGetIntersection(\_:otherRange:) 

Function

# CMTimeRangeGetIntersection(\_:otherRange:)

Returns a new time range with the time elements that are common between the input.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeGetIntersection(
    _ range: CMTimeRange,
    otherRange: CMTimeRange
) -> CMTimeRange
```

## Parameters 

`range`  

The first time range to intersect.

`otherRange`  

The second time range to intersect.

## Return Value

A time range that represents the largest intersection of the input.

## See Also

### Inspecting Time Ranges

func CMTIMERANGE_IS_EMPTY(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range has a duration of zero.

func CMTIMERANGE_IS_INDEFINITE(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range is indefinite.

func CMTIMERANGE_IS_INVALID(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range is invalid.

func CMTIMERANGE_IS_VALID(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range is valid.

func CMTimeRangeGetEnd(CMTimeRange) -> CMTime

Returns a time value that represents the end of a time range.

func CMTimeRangeGetUnion(CMTimeRange, otherRange: CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements of the input.

