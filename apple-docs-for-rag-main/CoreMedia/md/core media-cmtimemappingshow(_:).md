

- Core Media
-  CMTimeMappingShow(\_:) 

Function

# CMTimeMappingShow(\_:)

Prints a description of a time mapping to standard output.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingShow(_ mapping: CMTimeMapping)
```

## Parameters 

`mapping`  

The time mapping to show.

## Discussion

You typically use this function for debugging purposes.

## See Also

### Representing Time Mappings

func CMTimeMappingCopyAsDictionary(CMTimeMapping, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time mapping.

func CMTimeMappingCopyDescription(allocator: CFAllocator?, mapping: CMTimeMapping) -> CFString?

Copies a string description of a time mapping.

