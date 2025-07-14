

- Metal
- MTLRenderCommandEncoder
-  drawMeshThreads(\_:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:) 

Instance Method

# drawMeshThreads(\_:threadsPerObjectThreadgroup:threadsPerMeshThreadgroup:)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threads.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func drawMeshThreads(
    _ threadsPerGrid: MTLSize,
    threadsPerObjectThreadgroup: MTLSize,
    threadsPerMeshThreadgroup: MTLSize
)
```

**Required**

## Parameters 

`threadsPerGrid`  

An MTLSize instance that represents the number of threads for each grid dimension.

For mesh shaders, the command rounds the value down to the nearest multiple of `threadsPerMeshThreadgroup` for each dimension.

For object shaders, the value doesn’t need to be a multiple of `threadsPerObjectThreadgroup`.

`threadsPerObjectThreadgroup`  

An MTLSize instance that represents the number of threads in an object shader threadgroup, if applicable.

`threadsPerMeshThreadgroup`  

An MTLSize instance that represents the number of threads in a mesh shader threadgroup.

## See Also

### Drawing with Meshes

func drawMeshThreadgroups(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threadgroups.

**Required**

func drawMeshThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with indirect arguments.

**Required**

