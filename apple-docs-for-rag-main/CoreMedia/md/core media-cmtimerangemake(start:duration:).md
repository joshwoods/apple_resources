

- Core Media
-  CMTimeRangeMake(start:duration:) 

Function

# CMTimeRangeMake(start:duration:)

Creates a valid time range with a start time and duration.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeMake(
    start: CMTime,
    duration: CMTime
) -> CMTimeRange
```

## Parameters 

`start`  

The start of the time range.

`duration`  

The duration of the time range.

## Return Value

A valid time range structure, or an invalid time range if the duration’s epoch isn’t `0`.

## See Also

### Creating Time Ranges

func CMTimeRangeMakeFromDictionary(CFDictionary) -> CMTimeRange

Creates a time range from a dictionary representation of its fields.

func CMTimeRangeFromTimeToTime(start: CMTime, end: CMTime) -> CMTimeRange

Creates a valid time range from a start and end time.

