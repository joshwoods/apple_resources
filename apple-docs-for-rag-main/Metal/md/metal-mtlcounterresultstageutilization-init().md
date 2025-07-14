

- Metal
- MTLCounterResultStageUtilization
-  init() 

Initializer

# init()

Creates a default stage-utilization result.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init()
```

## Discussion

Metal creates MTLCounterResultStageUtilization instances for you when you resolve the counter set’s data (see Converting a GPU’s Counter Data into a Readable Format). There’s no reason for you to manually create one in your app.

## See Also

### Swift Support

init(totalCycles: UInt64, vertexCycles: UInt64, tessellationCycles: UInt64, postTessellationVertexCycles: UInt64, fragmentCycles: UInt64, renderTargetCycles: UInt64)

Creates a stage-utilization result from utilization values.

