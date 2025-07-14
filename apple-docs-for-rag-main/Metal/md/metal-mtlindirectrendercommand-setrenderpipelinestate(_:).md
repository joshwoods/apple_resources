

- Metal
- MTLIndirectRenderCommand
-  setRenderPipelineState(\_:) 

Instance Method

# setRenderPipelineState(\_:)

Sets the render pipeline state object used by the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
func setRenderPipelineState(_ pipelineState: any MTLRenderPipelineState)
```

**Required**

## Parameters 

`pipelineState`  

The rendering pipeline state object to use.

## Discussion

If you created the indirect command buffer with inheritPipelineState set to true, do not call this method. The command gets the pipeline state object from the parent encoder when you execute the command.

If you created the indirect command buffer with inheritPipelineState set to false, you must set the pipeline state prior to encoding the drawing command.

## See Also

### Setting Command Arguments

func setVertexBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a vertex buffer argument for the command.

**Required**

func setFragmentBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a fragment buffer argument for the command.

**Required**

