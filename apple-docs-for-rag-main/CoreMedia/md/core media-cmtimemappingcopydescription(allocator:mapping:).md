

- Core Media
-  CMTimeMappingCopyDescription(allocator:mapping:) 

Function

# CMTimeMappingCopyDescription(allocator:mapping:)

Copies a string description of a time mapping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingCopyDescription(
    allocator: CFAllocator?,
    mapping: CMTimeMapping
) -> CFString?
```

## Parameters 

`allocator`  

An allocator to use to create a dictionary. Pass `kCFAllocatorDefault` to use the default allocator.

`mapping`  

The time mapping from which to copy a description.

## Return Value

A string description of a time mapping.

## See Also

### Representing Time Mappings

func CMTimeMappingCopyAsDictionary(CMTimeMapping, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time mapping.

func CMTimeMappingShow(CMTimeMapping)

Prints a description of a time mapping to standard output.

