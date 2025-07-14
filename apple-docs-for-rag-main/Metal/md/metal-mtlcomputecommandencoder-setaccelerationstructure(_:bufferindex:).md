

- Metal
- MTLComputeCommandEncoder
-  setAccelerationStructure(\_:bufferIndex:) 

Instance Method

# setAccelerationStructure(\_:bufferIndex:)

Binds an acceleration structure to the buffer argument table, allowing functions to access it on the GPU.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setAccelerationStructure(
    _ accelerationStructure: (any MTLAccelerationStructure)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`accelerationStructure`  

An MTLAccelerationStructure instance to bind to the argument table.

`bufferIndex`  

The index the structure binds to in the argument table.

## See Also

### Encoding Acceleration Structures

func setIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Binds an intersection function table to the buffer argument table, making it callable in your Metal shaders.

**Required**

