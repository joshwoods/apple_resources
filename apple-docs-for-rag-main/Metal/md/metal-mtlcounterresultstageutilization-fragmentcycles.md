

- Metal
- MTLCounterResultStageUtilization
-  fragmentCycles 

Instance Property

# fragmentCycles

The number of cycles the GPU uses to run fragment shaders during a pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var fragmentCycles: UInt64
```

## See Also

### Stage Utilization Values

var totalCycles: UInt64

The total number of cycles the GPU uses to run a pass.

var vertexCycles: UInt64

The number of cycles the GPU uses to run vertex shaders during a pass.

var tessellationCycles: UInt64

The number of cycles the GPU uses to run the tessellation stage during a pass.

var postTessellationVertexCycles: UInt64

The number of cycles the GPU uses to run post-tessellation vertex shaders during a pass.

var renderTargetCycles: UInt64

The number of cycles the GPU uses to write data to render targets during a render pass.

