

- RealityKit
- LowLevelMesh
-  replace(bufferIndex:using:) 

Instance Method

# replace(bufferIndex:using:)

Retrieves a Metal vertex buffer you can use to replace the contents of the specified buffer on the GPU using Metal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func replace(
    bufferIndex index: Int,
    using commandBuffer: any MTLCommandBuffer
) -> any MTLBuffer
```

## Parameters 

`index`  

The index of the buffer to modify. Use a value that is less than vertexBufferCount.

`commandBuffer`  

The MTLCommandBuffer you intend to use for buffer modifications. RealityKit waits for the command buffer to complete before utilizing the buffer for rendering.

## Discussion

The buffer’s contents are in an uninitialized state.

## See Also

### Accessing mesh data on the GPU with Metal

func read(bufferIndex: Int, using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal vertex buffer at the specified index, for GPU reading.

func readIndices(using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves the Metal index buffer for GPU reading.

func replaceIndices(using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal index buffer that you can use to replace the indices of this low-level mesh.

