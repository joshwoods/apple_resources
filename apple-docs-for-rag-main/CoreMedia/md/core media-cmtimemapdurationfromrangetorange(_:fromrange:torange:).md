

- Core Media
-  CMTimeMapDurationFromRangeToRange(\_:fromRange:toRange:) 

Function

# CMTimeMapDurationFromRangeToRange(\_:fromRange:toRange:)

Translates a duration through a mapping from two time ranges.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMapDurationFromRangeToRange(
    _ dur: CMTime,
    fromRange: CMTimeRange,
    toRange: CMTimeRange
) -> CMTime
```

## Parameters 

`dur`  

The duration to translate.

`fromRange`  

The time range from which the function translates the duration.

`toRange`  

The time range to which the function maps the duration.

## Return Value

A time structure that represents the translated duration.

## Discussion

The function scales the duration in proportion to the ratio between the ranges’ durations:

```
result = dur*(toRange.duration/fromRange.duration)
```

If `dur` doesn’t have the epoch `0`, the function returns an invalid `CMTime`.

## See Also

### Utility Functions

func CMTimeClampToRange(CMTime, range: CMTimeRange) -> CMTime

Returns the nearest time value inside the time range.

func CMTimeMapTimeFromRangeToRange(CMTime, fromRange: CMTimeRange, toRange: CMTimeRange) -> CMTime

Translates a time through a mapping from two time ranges.

func CMTimeRangeCopyAsDictionary(CMTimeRange, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time range.

func CMTimeRangeCopyDescription(allocator: CFAllocator?, range: CMTimeRange) -> CFString?

Returns a string with a description of a time range.

func CMTimeRangeShow(CMTimeRange)

Prints a description of the time range to standard error.

