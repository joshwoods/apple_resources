

- Core Media
-  CMTimeMappingCopyAsDictionary(\_:allocator:) 

Function

# CMTimeMappingCopyAsDictionary(\_:allocator:)

Returns a dictionary representation of a time mapping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMappingCopyAsDictionary(
    _ mapping: CMTimeMapping,
    allocator: CFAllocator?
) -> CFDictionary?
```

## Parameters 

`mapping`  

The time mapping for which to create a dictionary representation.

`allocator`  

An allocator to use to create a dictionary. Pass `kCFAllocatorDefault` to use the default allocator.

## Return Value

A dictionary representation of a time mapping.

## See Also

### Representing Time Mappings

func CMTimeMappingCopyDescription(allocator: CFAllocator?, mapping: CMTimeMapping) -> CFString?

Copies a string description of a time mapping.

func CMTimeMappingShow(CMTimeMapping)

Prints a description of a time mapping to standard output.

