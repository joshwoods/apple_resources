

- Core Media
-  CMTimeRangeGetEnd(\_:) 

Function

# CMTimeRangeGetEnd(\_:)

Returns a time value that represents the end of a time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeGetEnd(_ range: CMTimeRange) -> CMTime
```

## Parameters 

`range`  

The time range from which to find the end of the time range.

## Return Value

A time structure.

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

func CMTimeRangeGetIntersection(CMTimeRange, otherRange: CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements that are common between the input.

func CMTimeRangeGetUnion(CMTimeRange, otherRange: CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements of the input.

