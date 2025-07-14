

- Core Media
-  CMTIMERANGE_IS_VALID(\_:) 

Function

# CMTIMERANGE_IS_VALID(\_:)

Returns a Boolean value that indicates whether a time range is valid.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTIMERANGE_IS_VALID(_ range: CMTimeRange) -> Bool
```

## Parameters 

`range`  

The time range.

## Return Value

true if `range` is valid; otherwise, false.

## See Also

### Inspecting Time Ranges

func CMTIMERANGE_IS_EMPTY(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range has a duration of zero.

func CMTIMERANGE_IS_INDEFINITE(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range is indefinite.

func CMTIMERANGE_IS_INVALID(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range is invalid.

func CMTimeRangeGetEnd(CMTimeRange) -> CMTime

Returns a time value that represents the end of a time range.

func CMTimeRangeGetIntersection(CMTimeRange, otherRange: CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements that are common between the input.

func CMTimeRangeGetUnion(CMTimeRange, otherRange: CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements of the input.

