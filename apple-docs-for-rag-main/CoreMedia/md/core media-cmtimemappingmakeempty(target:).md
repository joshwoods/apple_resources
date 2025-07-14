

- Core Media
-  CMTimeMappingMakeEmpty(target:) 

Function

# CMTimeMappingMakeEmpty(target:)

Creates a valid time mapping with an empty source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingMakeEmpty(target: CMTimeRange) -> CMTimeMapping
```

## Parameters 

`target`  

A time range on the target timeline.

## Return Value

A new time mapping.

## Discussion

The target time range must have a duration whose epoch is `0`, otherwise the system returns an invalid time mapping.

## See Also

### Creating Time Mappings

func CMTimeMappingMake(source: CMTimeRange, target: CMTimeRange) -> CMTimeMapping

Creates a time mapping with a source and target time range.

func CMTimeMappingMakeFromDictionary(CFDictionary) -> CMTimeMapping

Creates a time mapping from a dictionary representation.

