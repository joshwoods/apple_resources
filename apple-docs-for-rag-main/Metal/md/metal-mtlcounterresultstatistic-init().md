

- Metal
- MTLCounterResultStatistic
-  init() 

Initializer

# init()

Creates a default statistics result.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init()
```

## Discussion

Metal creates MTLCounterResultStatistic instances for you when you resolve the counter set’s data (see Converting a GPU’s Counter Data into a Readable Format). There’s no reason for you to manually create one in your app.

## See Also

### Swift Support

init(tessellationInputPatches: UInt64, vertexInvocations: UInt64, postTessellationVertexInvocations: UInt64, clipperInvocations: UInt64, clipperPrimitivesOut: UInt64, fragmentInvocations: UInt64, fragmentsPassed: UInt64, computeKernelInvocations: UInt64)

Creates a statistics result from statistic values.

