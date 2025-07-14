

- Metal
- MTLIndirectRenderCommand
-  setFragmentBuffer(\_:offset:at:) 

Instance Method

# setFragmentBuffer(\_:offset:at:)

Sets a fragment buffer argument for the command.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func setFragmentBuffer(
    _ buffer: any MTLBuffer,
    offset: Int,
    at index: Int
)
```

**Required**

## Parameters 

`buffer`  

The buffer to set in the buffer argument table.

`offset`  

The location, in bytes relative to start of `buffer`, of the first byte of data for the fragment shader.

`index`  

An index in the buffer argument table. The maximum index is determined when you created the indirect command buffer.

## Discussion

If you created the indirect command buffer with inheritBuffers set to true, do not call this method. The command gets the arguments from the parent encoder when you execute the command.

If you need to pass other kinds of parameters to your shader, such as textures and samplers, create an argument buffer and pass it to the shader using this method.

## See Also

### Setting Command Arguments

func setRenderPipelineState(any MTLRenderPipelineState)

Sets the render pipeline state object used by the command.

**Required**

func setVertexBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a vertex buffer argument for the command.

**Required**

