

- Metal
- MTLRenderCommandEncoder
-  drawMeshThreadgroups(indirectBuffer:indirectBufferOffset:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:) 

Instance Method

# drawMeshThreadgroups(indirectBuffer:indirectBufferOffset:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with indirect arguments.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func drawMeshThreadgroups(
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int,
    threadsPerObjectThreadgroup: MTLSize,
    threadsPerMeshThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`indirectBuffer`  

An MTLBuffer instance with data that matches the layout of the MTLDispatchThreadgroupsIndirectArguments structure.

`indirectBufferOffset`  

An integer that represents the location, in bytes, from the start of `indirectBuffer` where the indirect arguments structure begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

`threadsPerObjectThreadgroup`  

An MTLSize instance that represents the number of threads in an object shader threadgroup, if applicable.

`threadsPerMeshThreadgroup`  

An MTLSize instance that represents the number of threads in a mesh shader threadgroup.

## See Also

### Drawing with Meshes

func drawMeshThreads(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threads.

**Required**

func drawMeshThreadgroups(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threadgroups.

**Required**

