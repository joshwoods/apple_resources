

- Metal
- MTLRenderCommandEncoder
-  setFragmentAccelerationStructure(\_:bufferIndex:) 

Instance Method

# setFragmentAccelerationStructure(\_:bufferIndex:)

Assigns an acceleration structure to an entry in the fragment shader argument table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func setFragmentAccelerationStructure(
    _ accelerationStructure: (any MTLAccelerationStructure)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`accelerationStructure`  

An MTLAccelerationStructure instance the command assigns to an entry in the fragment shader argument table for acceleration structures.

`bufferIndex`  

An integer that represents the entry in the fragment shader argument table for acceleration structures that stores a record of `accelerationStructure`.

## Discussion

By default, the acceleration structure at each index is `nil`.

