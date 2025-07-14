

- Metal
- MTLComputePipelineState
-  imageblockMemoryLength(forDimensions:) 

Instance Method

# imageblockMemoryLength(forDimensions:)

Returns the length of reserved memory for an imageblock of a given size.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func imageblockMemoryLength(forDimensions imageblockDimensions: MTLSize) -> Int
```

**Required**

## Parameters 

`imageblockDimensions`  

An MTLSize instance that represents the dimensions of an imageblock.

## Return Value

The length, in bytes, occupied by the image block in memory.

