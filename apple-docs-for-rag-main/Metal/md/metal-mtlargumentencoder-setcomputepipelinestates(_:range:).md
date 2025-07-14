

- Metal
- MTLArgumentEncoder
-  setComputePipelineStates(\_:range:) 

Instance Method

# setComputePipelineStates(\_:range:)

Encodes references to an array of compute pipeline states into the argument buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS

``` source
func setComputePipelineStates(
    _ pipelines: [(any MTLComputePipelineState)?],
    range: Range
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

func setComputePipelineStates(UnsafePointer&lt;(any MTLComputePipelineState)?>, with: NSRange)

Encodes references to an array of compute pipeline states into the argument buffer.

func setComputePipelineState((any MTLComputePipelineState)?, at: Int)

Encodes a reference to a compute pipeline state into the argument buffer.

