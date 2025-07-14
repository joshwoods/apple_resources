

- Metal
- MTLCommonCounter
-  timestamp 

Type Property

# timestamp

The common name for the counter that tracks the current time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let timestamp: MTLCommonCounter
```

## See Also

### Common Counter Names

static let tessellationInputPatches: MTLCommonCounter

The common name for the counter that tracks the number of tessellation patches a render pass sends to the tessellation stage.

static let vertexInvocations: MTLCommonCounter

The common name for the counter that tracks the number of times a render pass calls any vertex shader.

static let postTessellationVertexInvocations: MTLCommonCounter

The common name for the counter that tracks the number of vertices a render pass sends to a post-tessellation vertex shader.

static let clipperInvocations: MTLCommonCounter

The common name for the counter that tracks the number of primitives a render pass sends to the clip stage.

static let clipperPrimitivesOut: MTLCommonCounter

The common name for the counter that tracks the number of primitives the clip stage produces during a render pass.

static let fragmentInvocations: MTLCommonCounter

The common name for the counter that tracks the number of times a render pass calls fragment shaders.

static let fragmentsPassed: MTLCommonCounter

The common name for the counter that tracks the number of fragments a render pass sends to the visibility and blend stages.

static let computeKernelInvocations: MTLCommonCounter

The common name for the counter that tracks the number of times a pass invokes any compute kernel.

static let totalCycles: MTLCommonCounter

The common name for the counter that tracks the total number of cycles the GPU uses to run a pass.

static let vertexCycles: MTLCommonCounter

The common name for the counter that tracks the number of cycles the GPU uses to run vertex shaders during a pass.

static let postTessellationVertexCycles: MTLCommonCounter

The common name for the counter that tracks the number of cycles the GPU uses to run post-tessellation vertex shaders during a pass.

static let fragmentCycles: MTLCommonCounter

The common name for the counter that tracks the number of cycles the GPU uses to run fragment shaders during a pass.

static let tessellationCycles: MTLCommonCounter

The common name for the counter that tracks the number of cycles the GPU uses to run the tessellation stage during a pass.

static let renderTargetWriteCycles: MTLCommonCounter

The common name for the counter that tracks the number of cycles the GPU uses to write data to render targets during a render pass.

