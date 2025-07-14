

- Core Media
-  CMTimeClampToRange(\_:range:) 

Function

# CMTimeClampToRange(\_:range:)

Returns the nearest time value inside the time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeClampToRange(
    _ time: CMTime,
    range: CMTimeRange
) -> CMTime
```

## Parameters 

`time`  

The time to clamp.

`range`  

The time range to examine.

## Return Value

A time structure inside the time range.

## Discussion

The function returns the times inside the range you specify unmodified. Times before the start and after the end time of the time range return the start and end time of the range. If the `CMTimeRange` argument is empty, this function returns an invalid `CMTime`. If the given `CMTime` is invalid, the function returns an invalid `CMTime`.

## See Also

### Utility Functions

func CMTimeMapDurationFromRangeToRange(CMTime, fromRange: CMTimeRange, toRange: CMTimeRange) -> CMTime

Translates a duration through a mapping from two time ranges.

func CMTimeMapTimeFromRangeToRange(CMTime, fromRange: CMTimeRange, toRange: CMTimeRange) -> CMTime

Translates a time through a mapping from two time ranges.

func CMTimeRangeCopyAsDictionary(CMTimeRange, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time range.

func CMTimeRangeCopyDescription(allocator: CFAllocator?, range: CMTimeRange) -> CFString?

Returns a string with a description of a time range.

func CMTimeRangeShow(CMTimeRange)

Prints a description of the time range to standard error.

