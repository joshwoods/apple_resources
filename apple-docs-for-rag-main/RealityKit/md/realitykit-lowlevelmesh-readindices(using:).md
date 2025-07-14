

- RealityKit
- LowLevelMesh
-  readIndices(using:) 

Instance Method

# readIndices(using:)

Retrieves the Metal index buffer for GPU reading.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func readIndices(using commandBuffer: any MTLCommandBuffer) -> any MTLBuffer
```

## Parameters 

`commandBuffer`  

The MTLCommandBuffer you intend to use for reading. RealityKit waits for the command buffer to complete before discarding the buffer.

## See Also

### Accessing mesh data on the GPU with Metal

func read(bufferIndex: Int, using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal vertex buffer at the specified index, for GPU reading.

func replace(bufferIndex: Int, using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal vertex buffer you can use to replace the contents of the specified buffer on the GPU using Metal.

func replaceIndices(using: any MTLCommandBuffer) -> any MTLBuffer

Retrieves a Metal index buffer that you can use to replace the indices of this low-level mesh.

