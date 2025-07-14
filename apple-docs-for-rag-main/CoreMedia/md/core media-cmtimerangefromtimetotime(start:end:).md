

- Core Media
-  CMTimeRangeFromTimeToTime(start:end:) 

Function

# CMTimeRangeFromTimeToTime(start:end:)

Creates a valid time range from a start and end time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeFromTimeToTime(
    start: CMTime,
    end: CMTime
) -> CMTimeRange
```

## Parameters 

`start`  

The start time of the range.

`end`  

The end time of the range.

## Return Value

A valid time range structure.

## See Also

### Creating Time Ranges

func CMTimeRangeMake(start: CMTime, duration: CMTime) -> CMTimeRange

Creates a valid time range with a start time and duration.

func CMTimeRangeMakeFromDictionary(CFDictionary) -> CMTimeRange

Creates a time range from a dictionary representation of its fields.

