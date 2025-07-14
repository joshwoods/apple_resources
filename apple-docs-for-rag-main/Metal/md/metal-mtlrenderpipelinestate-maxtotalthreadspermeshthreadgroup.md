

- Metal
- MTLRenderPipelineState
-  maxTotalThreadsPerMeshThreadgroup 

Instance Property

# maxTotalThreadsPerMeshThreadgroup

The largest number of threads the pipeline state can have in a single mesh shader threadgroup.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var maxTotalThreadsPerMeshThreadgroup: Int { get }
```

**Required**

## See Also

### Checking Mesh Shader Memory Requirements

var maxTotalThreadgroupsPerMeshGrid: Int

The largest number of threadgroups the pipeline state can have in a single mesh shader grid.

**Required**

var meshThreadExecutionWidth: Int

The number of threads the render pass applies to a SIMD group for a mesh shader.

**Required**

