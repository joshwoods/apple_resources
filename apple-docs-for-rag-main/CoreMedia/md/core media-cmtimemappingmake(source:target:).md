

- Core Media
-  CMTimeMappingMake(source:target:) 

Function

# CMTimeMappingMake(source:target:)

Creates a time mapping with a source and target time range.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingMake(
    source: CMTimeRange,
    target: CMTimeRange
) -> CMTimeMapping
```

## Parameters 

`source`  

A time range on the source timeline.

`target`  

A time range on the target timeline.

## Return Value

A new time mapping.

## Discussion

The source and target parameters must have durations whose epoch is `0`, otherwise the system returns an invalid time mapping.

## See Also

### Creating Time Mappings

func CMTimeMappingMakeEmpty(target: CMTimeRange) -> CMTimeMapping

Creates a valid time mapping with an empty source.

func CMTimeMappingMakeFromDictionary(CFDictionary) -> CMTimeMapping

Creates a time mapping from a dictionary representation.

