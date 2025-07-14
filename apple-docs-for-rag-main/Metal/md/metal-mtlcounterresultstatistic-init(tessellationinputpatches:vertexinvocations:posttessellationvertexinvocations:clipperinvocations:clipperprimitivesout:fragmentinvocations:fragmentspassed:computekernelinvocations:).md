

- Metal
- MTLCounterResultStatistic
-  init(tessellationInputPatches:vertexInvocations:postTessellationVertexInvocations:clipperInvocations:clipperPrimitivesOut:fragmentInvocations:fragmentsPassed:computeKernelInvocations:) 

Initializer

# init(tessellationInputPatches:vertexInvocations:postTessellationVertexInvocations:clipperInvocations:clipperPrimitivesOut:fragmentInvocations:fragmentsPassed:computeKernelInvocations:)

Creates a statistics result from statistic values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    tessellationInputPatches: UInt64,
    vertexInvocations: UInt64,
    postTessellationVertexInvocations: UInt64,
    clipperInvocations: UInt64,
    clipperPrimitivesOut: UInt64,
    fragmentInvocations: UInt64,
    fragmentsPassed: UInt64,
    computeKernelInvocations: UInt64
)
```

## Parameters 

`tessellationInputPatches`  

The number of tessellation patches the render pass sends to the tessellation stage.

`vertexInvocations`  

The number of times the render pass calls vertex shaders.

`postTessellationVertexInvocations`  

The number of vertices the tessellation stage creates.

`clipperInvocations`  

The number of primitives the clip stage consumes.

`clipperPrimitivesOut`  

The number of primitives the clip stage produces.

`fragmentInvocations`  

The number of times the render pass calls fragment shaders.

`fragmentsPassed`  

The number of fragments the render pass sends to the visibility and blend stages.

`computeKernelInvocations`  

The number of times the pass calls compute kernels.

## Discussion

Metal creates MTLCounterResultStatistic instances for you when you resolve the counter set’s data (see Converting a GPU’s Counter Data into a Readable Format). There’s no reason for you to manually create one in your app.

## See Also

### Swift Support

init()

Creates a default statistics result.

