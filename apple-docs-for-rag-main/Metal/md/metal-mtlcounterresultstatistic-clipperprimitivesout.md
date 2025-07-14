

- Metal
- MTLCounterResultStatistic
-  clipperPrimitivesOut 

Instance Property

# clipperPrimitivesOut

The number of primitives the clip stage produces during a render pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var clipperPrimitivesOut: UInt64
```

## See Also

### Statistics Values

var tessellationInputPatches: UInt64

The number of tessellation patches a render pass sends to the tessellation stage.

var vertexInvocations: UInt64

The number of times a render pass calls any vertex shader.

var postTessellationVertexInvocations: UInt64

The number of vertices a render pass sends to a post-tessellation vertex shader.

var clipperInvocations: UInt64

The number of primitives a render pass sends to the clip stage.

var fragmentInvocations: UInt64

The number of times a render pass calls fragment shaders.

var fragmentsPassed: UInt64

The number of fragments a render pass sends to the visibility and blend stages because they pass the scissor, depth, and stencil tests.

var computeKernelInvocations: UInt64

The number of times a pass calls any compute kernel.

