

- Core Media
-  CMTimeCopyAsDictionary(\_:allocator:) 

Function

# CMTimeCopyAsDictionary(\_:allocator:)

Creates a dictionary representation of the time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeCopyAsDictionary(
    _ time: CMTime,
    allocator: CFAllocator?
) -> CFDictionary?
```

## Parameters 

`time`  

A time from which to create a dictionary.

`allocator`  

An allocator with which to create the dictionary. Pass kCFAllocatorDefault to use the default allocator.

## Return Value

A dictionary representation of the time.

## See Also

### Representing Times

func CMTimeShow(CMTime)

Prints a description of the time to the console.

func CMTimeCopyDescription(allocator: CFAllocator?, time: CMTime) -> CFString?

Creates a string representation of the time.

