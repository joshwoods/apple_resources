

- Core Media
-  CMTimeCopyDescription(allocator:time:) 

Function

# CMTimeCopyDescription(allocator:time:)

Creates a string representation of the time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeCopyDescription(
    allocator: CFAllocator?,
    time: CMTime
) -> CFString?
```

## Parameters 

`allocator`  

An allocator with which to create the description. Pass kCFAllocatorDefault to use the default allocator.

`time`  

The time to describe.

## Return Value

A string representation of the time.

## See Also

### Representing Times

func CMTimeShow(CMTime)

Prints a description of the time to the console.

func CMTimeCopyAsDictionary(CMTime, allocator: CFAllocator?) -> CFDictionary?

Creates a dictionary representation of the time.

