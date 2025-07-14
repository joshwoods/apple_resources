

- Core Media
-  CMTimeMappingMakeFromDictionary(\_:) 

Function

# CMTimeMappingMakeFromDictionary(\_:)

Creates a time mapping from a dictionary representation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingMakeFromDictionary(_ dictionaryRepresentation: CFDictionary) -> CMTimeMapping
```

## Parameters 

`dictionaryRepresentation`  

A dictionary representation of a time mapping that you previously created by calling the CMTimeMappingCopyAsDictionary(_:allocator:) function.

## Return Value

A new time mapping.

## Discussion

If the dictionary you provide doesn’t have the requisite keyed values, the system returns an invalid time mapping.

## See Also

### Creating Time Mappings

func CMTimeMappingMake(source: CMTimeRange, target: CMTimeRange) -> CMTimeMapping

Creates a time mapping with a source and target time range.

func CMTimeMappingMakeEmpty(target: CMTimeRange) -> CMTimeMapping

Creates a valid time mapping with an empty source.

