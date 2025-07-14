

- Core Media
-  CMTimeShow(\_:) 

Function

# CMTimeShow(\_:)

Prints a description of the time to the console.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeShow(_ time: CMTime)
```

## Parameters 

`time`  

A time to show.

## Discussion

This function is most appropriate to use for debugging purposes.

## See Also

### Representing Times

func CMTimeCopyDescription(allocator: CFAllocator?, time: CMTime) -> CFString?

Creates a string representation of the time.

func CMTimeCopyAsDictionary(CMTime, allocator: CFAllocator?) -> CFDictionary?

Creates a dictionary representation of the time.

