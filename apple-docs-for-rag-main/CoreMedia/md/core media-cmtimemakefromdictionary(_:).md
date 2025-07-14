

- Core Media
-  CMTimeMakeFromDictionary(\_:) 

Function

# CMTimeMakeFromDictionary(\_:)

Creates a time from a dictionary representation of its fields.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMakeFromDictionary(_ dictionaryRepresentation: CFDictionary?) -> CMTime
```

## Parameters 

`dictionaryRepresentation`  

A dictionary created from a call to CMTimeCopyAsDictionary(_:allocator:).

## Return Value

A time structure.

## Discussion

For keys in the dictionary, see Dictionary Keys.

## See Also

### Creating a Time

func CMTimeMake(value: Int64, timescale: Int32) -> CMTime

Creates a time with a value and timescale.

func CMTimeMakeWithEpoch(value: Int64, timescale: Int32, epoch: Int64) -> CMTime

Creates a time with a value, timescale, and epoch.

func CMTimeMakeWithSeconds(Float64, preferredTimescale: Int32) -> CMTime

Creates a time that represents a number of seconds in a preferred timescale.

