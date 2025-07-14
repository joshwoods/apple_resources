

- Metal
- MTLRenderCommandEncoder
-  drawMeshThreadgroups(\_:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:) 

Instance Method

# drawMeshThreadgroups(\_:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threadgroups.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func drawMeshThreadgroups(
    _ threadgroupsPerGrid: MTLSize,
    threadsPerObjectThreadgroup: MTLSize,
    threadsPerMeshThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`threadgroupsPerGrid`  

An MTLSize instance that represents the number of threadgroups for each grid dimension.

`threadsPerObjectThreadgroup`  

An MTLSize instance that represents the number of threads in an object shader threadgroup, if applicable.

`threadsPerMeshThreadgroup`  

An MTLSize instance that represents the number of threads in a mesh shader threadgroup.

## See Also

### Drawing with Meshes

func drawMeshThreads(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threads.

**Required**

func drawMeshThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with indirect arguments.

**Required**

