

- Core Media
-  CMTimeRangeCopyDescription(allocator:range:) 

Function

# CMTimeRangeCopyDescription(allocator:range:)

Returns a string with a description of a time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeCopyDescription(
    allocator: CFAllocator?,
    range: CMTimeRange
) -> CFString?
```

## Parameters 

`allocator`  

The allocator the function uses when allocating memory for the description.

`range`  

The time range to describe.

## Return Value

A string description.

## Discussion

You use this from within `CFShow` on an object that contains `CMTimeRange` fields. It is also useful from other client debugging code. The caller owns the `CFString` this function returns and is responsible for releasing it. Pass `kCFAllocatorDefault` to use the default allocator.

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

func CMTimeRangeShow(CMTimeRange)

Prints a description of the time range to standard error.

