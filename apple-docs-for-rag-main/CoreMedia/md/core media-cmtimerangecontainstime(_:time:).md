

- Core Media
-  CMTimeRangeContainsTime(\_:time:) 

Function

# CMTimeRangeContainsTime(\_:time:)

Returns a Boolean value that indicates whether a time range contains a time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeContainsTime(
    _ range: CMTimeRange,
    time: CMTime
) -> Bool
```

## Parameters 

`range`  

A time range.

`time`  

A time value to test for in the time range.

## Return Value

true if `range` contains the `time` value; otherwise, false.

## See Also

### Comparing Time Ranges

func CMTimeRangeEqual(CMTimeRange, CMTimeRange) -> Bool

Returns a Boolean value that indicates whether two time ranges are equal.

func CMTimeRangeContainsTimeRange(CMTimeRange, otherRange: CMTimeRange) -> Bool

Returns a Boolean value that indicates whether a time range contains another time range.

