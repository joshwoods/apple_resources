

- Metal
- MTLArgumentEncoder
-  setComputePipelineStates(\_:with:) 

Instance Method

# setComputePipelineStates(\_:with:)

Encodes references to an array of compute pipeline states into the argument buffer.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedmacOS 10.13+tvOS 13.0–14.0DeprecatedvisionOS

``` source
func setComputePipelineStates(
    _ pipelines: UnsafePointer,
    with range: NSRange
)
```

## Parameters 

`pipelines`  

An array of pipeline states the method encodes.

`range`  

A range of indices within the argument buffer for each element in `pipelines`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

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

func setComputePipelineState((any MTLComputePipelineState)?, at: Int)

Encodes a reference to a compute pipeline state into the argument buffer.

func setComputePipelineStates([(any MTLComputePipelineState)?], range: Range&lt;Int>)

Encodes references to an array of compute pipeline states into the argument buffer.

