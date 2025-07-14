

- Core Media
-  CMTimeRangeShow(\_:) 

Function

# CMTimeRangeShow(\_:)

Prints a description of the time range to standard error.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeShow(_ range: CMTimeRange)
```

## Parameters 

`range`  

The time range to print.

## Discussion

This is most useful from within LLDB.

## See Also

### Utility Functions

func CMTimeClampToRange(CMTime, range: CMTimeRange) -> CMTime

Returns the nearest time value inside the time range.

func CMTimeMapDurationFromRangeToRange(CMTime, fromRange: CMTimeRange, toRange: CMTimeRange) -> CMTime

Translates a duration through a mapping from two time ranges.

func CMTimeMapTimeFromRangeToRange(CMTime, fromRange: CMTimeRange, toRange: CMTimeRange) -> CMTime

Translates a time through a mapping from two time ranges.

func CMTimeRangeCopyAsDictionary(CMTimeRange, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time range.

func CMTimeRangeCopyDescription(allocator: CFAllocator?, range: CMTimeRange) -> CFString?

Returns a string with a description of a time range.

