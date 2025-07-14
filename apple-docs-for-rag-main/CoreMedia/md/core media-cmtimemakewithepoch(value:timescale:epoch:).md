

- Core Media
-  CMTimeMakeWithEpoch(value:timescale:epoch:) 

Function

# CMTimeMakeWithEpoch(value:timescale:epoch:)

Creates a time with a value, timescale, and epoch.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMakeWithEpoch(
    value: Int64,
    timescale: Int32,
    epoch: Int64
) -> CMTime
```

## Parameters 

`value`  

An integer time value.

`timescale`  

An integer timescale value.

`epoch`  

An integer epoch value.

## Return Value

A time structure.

## See Also

### Creating a Time

func CMTimeMake(value: Int64, timescale: Int32) -> CMTime

Creates a time with a value and timescale.

func CMTimeMakeWithSeconds(Float64, preferredTimescale: Int32) -> CMTime

Creates a time that represents a number of seconds in a preferred timescale.

func CMTimeMakeFromDictionary(CFDictionary?) -> CMTime

Creates a time from a dictionary representation of its fields.

