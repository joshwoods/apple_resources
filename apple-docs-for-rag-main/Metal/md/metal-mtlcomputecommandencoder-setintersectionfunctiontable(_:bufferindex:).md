

- Metal
- MTLComputeCommandEncoder
-  setIntersectionFunctionTable(\_:bufferIndex:) 

Instance Method

# setIntersectionFunctionTable(\_:bufferIndex:)

Binds an intersection function table to the buffer argument table, making it callable in your Metal shaders.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setIntersectionFunctionTable(
    _ intersectionFunctionTable: (any MTLIntersectionFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`intersectionFunctionTable`  

The MTLIntersectionFunctionTable to bind.

`bufferIndex`  

The index in the buffer argument table the intersection function table binds to.

## See Also

### Encoding Acceleration Structures

func setAccelerationStructure((any MTLAccelerationStructure)?, bufferIndex: Int)

Binds an acceleration structure to the buffer argument table, allowing functions to access it on the GPU.

**Required**

