

- Metal
- MTLCounterResultStageUtilization
-  init(totalCycles:vertexCycles:tessellationCycles:postTessellationVertexCycles:fragmentCycles:renderTargetCycles:) 

Initializer

# init(totalCycles:vertexCycles:tessellationCycles:postTessellationVertexCycles:fragmentCycles:renderTargetCycles:)

Creates a stage-utilization result from utilization values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    totalCycles: UInt64,
    vertexCycles: UInt64,
    tessellationCycles: UInt64,
    postTessellationVertexCycles: UInt64,
    fragmentCycles: UInt64,
    renderTargetCycles: UInt64
)
```

## Parameters 

`totalCycles`  

The number of GPU cycles the entire render pass takes to run.

`vertexCycles`  

The number of GPU cycles the vertex shaders take to run.

`tessellationCycles`  

The number of GPU cycles the tessellating patches take to run.

`postTessellationVertexCycles`  

The number of GPU cycles the post-tessellation vertex shaders take to run.

`fragmentCycles`  

The number of GPU cycles the fragment shaders take to run.

`renderTargetCycles`  

The number of GPU cycles the pass takes writing data to render targets.

## Discussion

Metal creates MTLCounterResultStageUtilization instances for you when you resolve the counter set’s data (see Converting a GPU’s Counter Data into a Readable Format). There’s no reason for you to manually create one in your app.

## See Also

### Swift Support

init()

Creates a default stage-utilization result.

