

- Metal
- MTLArgumentEncoder
-  setComputePipelineState(\_:at:) 

Instance Method

# setComputePipelineState(\_:at:)

Encodes a reference to a compute pipeline state into the argument buffer.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedmacOS 10.13+tvOS 13.0–14.0DeprecatedvisionOS

``` source
func setComputePipelineState(
    _ pipeline: (any MTLComputePipelineState)?,
    at index: Int
)
```

## Parameters 

`pipeline`  

A pipeline state the method encodes.

`index`  

The index of a pipeline state within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Pipeline States

func setRenderPipelineState((any MTLRenderPipelineState)?, index: Int)

Encodes a reference to a render pipeline state into the argument buffer.

**Required**

func setRenderPipelineStates([(any MTLRenderPipelineState)?], range: Range&lt;Int>)

Encodes references to an array of render pipeline states into the argument buffer.

func setComputePipelineState((any MTLComputePipelineState)?, index: Int)

Encodes a reference to a compute pipeline state into the argument buffer.

**Required**

func setComputePipelineStates(UnsafePointer&lt;(any MTLComputePipelineState)?>, with: NSRange)

Encodes references to an array of compute pipeline states into the argument buffer.

func setComputePipelineStates([(any MTLComputePipelineState)?], range: Range&lt;Int>)

Encodes references to an array of compute pipeline states into the argument buffer.

