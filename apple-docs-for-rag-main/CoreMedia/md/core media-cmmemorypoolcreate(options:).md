

- Core Media
-  CMMemoryPoolCreate(options:) 

Function

# CMMemoryPoolCreate(options:)

Creates a memory pool.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMemoryPoolCreate(options: CFDictionary?) -> CMMemoryPool
```

## Parameters 

`options`  

A dictionary that defines the age-out period for the pool.

## Return Value

A new memory pool.

## Topics

### Creation Options

let kCMMemoryPoolOption_AgeOutPeriod: CFString

The period of time before the pool recycles its memory.

