

- Core Media
-  CMTimeRangeMakeFromDictionary(\_:) 

Function

# CMTimeRangeMakeFromDictionary(\_:)

Creates a time range from a dictionary representation of its fields.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeRangeMakeFromDictionary(_ dictionaryRepresentation: CFDictionary) -> CMTimeRange
```

## Parameters 

`dictionaryRepresentation`  

A dictionary from which to create the time range.

## Return Value

A valid time range structure, or an invalid time range if `dict` doesn’t have the necessary values.

## Discussion

This is useful when getting Core Media time ranges from Core Foundation container types. For keys in the dictionary, see Dictionary Keys.

## See Also

### Creating Time Ranges

func CMTimeRangeMake(start: CMTime, duration: CMTime) -> CMTimeRange

Creates a valid time range with a start time and duration.

func CMTimeRangeFromTimeToTime(start: CMTime, end: CMTime) -> CMTimeRange

Creates a valid time range from a start and end time.

