

- Metal
- Resource Fundamentals
-  Synchronizing a Managed Resource in macOS 

Article

# Synchronizing a Managed Resource in macOS

Manually synchronize memory for a Metal resource in apps.

## Overview

For Mac computers with Intel or external GPUs, Metal offers *managed resources.* Managed resources are MTLResource instances, such as an MTLTexture or MTLBuffer, which use memory that your app can copy between the CPU and GPU. Managed resources use a storageMode of MTLStorageMode.managed.

You need to manually synchronize managed resources, copying changed memory between the CPU and GPU. This is different from Apple family GPUs, which use MTLStorageMode.shared for resources that the CPU and GPU can both access. Synchronize after your code finishes memory writes. After data synchronizes, you can safely read it in both your app and GPU functions.

As a best practice, try to keep your data synchronization points to a minimum. Even synchronization calls which don’t copy data can result in a small performance hit.

Note

Managed resources are the default memory storage type for Intel and external GPU devices in Metal. For more information about macOS resource storage modes and how to select them, see Choosing a Resource Storage Mode for Intel and AMD GPUs.

### Synchronize a Managed Buffer

First, create an MTLBuffer with the option MTLStorageMode.managed, which tells Metal to reserve managed memory space for the resource:

- Swift
- Objective-C

```
// Create a matrix data structure.
struct MatrixData {
    var modelMatrix = matrix_float4x4()
    var viewMatrix = matrix_float4x4()
    var projectionMatrix = matrix_float4x4()
}

// Create a managed buffer.
guard let matrixBuffer = device.makeBuffer(length: MemoryLayout.size, options: .storageModeManaged) else { return }
```

```
// Create a matrix data structure.
id  _matrixBuffer;
typedef struct
{
    matrix_float4x4 modelMatrix;
    matrix_float4x4 viewMatrix;
    matrix_float4x4 projectionMatrix;
} MatrixData;

// Create a managed buffer.
_matrixBuffer = [_device newBufferWithLength:sizeof(MatrixData)
                                     options:MTLResourceStorageModeManaged];
```

Next, modify the buffer’s data on the CPU:

- Swift
- Objective-C

```
// Modify the managed buffer's data with the CPU.
var matrixData = MatrixData()
matrixData.modelMatrix = updatedModelMatrix
matrixBuffer.contents().storeBytes(of: matrixData, as: MatrixData.self)
```

```
// Modify the managed buffer's data with the CPU.
MatrixData *matrixData = (MatrixData*)_matrixBuffer.contents;
matrixData->modelMatrix = updatedModelMatrix;
```

After completing a CPU modification, call the didModifyRange: method. This method updates a specific range of data and keeps the buffer synchronized. Before calling this method, the modified buffer’s data on the GPU is in an undefined state.

- Swift
- Objective-C

```
// Synchronize the managed buffer.
matrixBuffer.didModifyRange(0...size)
```

```
// Synchronize the managed buffer.
[_matrixBuffer didModifyRange:NSMakeRange(0, sizeof(matrixData->modelMatrix))];
```

After encoding a GPU modification, encode a synchronize(resource:) command. This command updates the entire buffer and keeps it synchronized. Before executing this command, the modified buffer’s data on the CPU is in an undefined state.

- Swift
- Objective-C

```
// Create a command buffer for GPU work.
if let commandBuffer = commandQueue.makeCommandBuffer() {
    // Create a compute command encoder.
    guard let computeCommandEncoder =
            commandBuffer.makeComputeCommandEncoder(dispatchType: MTLDispatchType.serial)
    else { return }

    // Encode a compute pass to modify the managed buffer's data with the GPU.
    computeCommandEncoder.setComputePipelineState(computePipelineStateObject)
    computeCommandEncoder.setBuffer(matrixBuffer, offset: 0, index: 0)
    computeCommandEncoder.dispatchThreads(gridSize, threadsPerThreadgroup: threadgroupSize)
    computeCommandEncoder.endEncoding()

    // Add a completion handler and commit the command buffer.
    let commandBufferHandler: MTLCommandBufferHandler
    commandBuffer.addCompletedHandler(commandBufferHandler)
    commandBuffer.commit()
}
```

```
// Create a command buffer for GPU work.
id  commandBuffer = [_commandQueue commandBuffer];

// Encode a compute pass to modify the managed buffer's data with the GPU.
id  computeCommandEncoder = [commandBuffer computeCommandEncoderWithDispatchType:MTLDispatchTypeSerial];
[computeCommandEncoder setComputePipelineState:computePipelineStateObject];
[computeCommandEncoder setBuffer:_matrixBuffer
                          offset:0
                         atIndex:0];
[computeCommandEncoder dispatchThreads:gridSize
                 threadsPerThreadgroup:threadgroupSize];
[computeCommandEncoder endEncoding];

// Synchronize the managed buffer.
id  blitCommandEncoder = [commandBuffer blitCommandEncoder];
[blitCommandEncoder synchronizeResource:_matrixBuffer];
[blitCommandEncoder endEncoding];

// Add a completion handler and commit the command buffer.
[commandBuffer addCompletedHandler:^(id cb) {
    // In this code block, the command buffer `cb` is updated and synchronized, and can be safely read or written to.
}];
[commandBuffer commit];
```

### Synchronize a Managed Texture

First, create an MTLTexture in managed memory from an MTLTextureDescriptor with its storage mode set to MTLStorageMode.managed:

- Swift
- Objective-C

```
// Create a texture descriptor.
let textureDescriptor = MTLTextureDescriptor.texture2DDescriptor(pixelFormat: .rgba8Unorm,
                                                                 width: textureSize.width,
                                                                 height: textureSize.height,
                                                                 mipmapped: false)

// Set the descriptor's storage mode and usage.
textureDescriptor.storageMode = MTLStorageMode.managed
textureDescriptor.usage = [.shaderRead, .shaderWrite]

// Create a managed texture.
let imageTexture = device.makeTexture(descriptor: textureDescriptor)
```

```
id  _imageTexture;
// Create a texture descriptor.
MTLTextureDescriptor *textureDescriptor = [MTLTextureDescriptor texture2DDescriptorWithPixelFormat:MTLPixelFormatRGBA8Unorm
                                                                                             width:textureSize.width
                                                                                            height:textureSize.height
                                                                                         mipmapped:NO];

// Set the descriptor's storage mode and usage.
textureDescriptor.storageMode = MTLStorageModeManaged;
textureDescriptor.usage = MTLTextureUsageShaderRead | MTLTextureUsageShaderWrite;

// Create a managed texture.
_imageTexture = [_device newTextureWithDescriptor:textureDescriptor];
```

To perform a CPU modification and simultaneously notify Metal about the change, call the replace(region:mipmapLevel:withBytes:bytesPerRow:) method. This method updates a specific region of data and keeps the texture synchronized. To update a specific texture slice, call the replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) method instead. Before calling one of these methods, the modified texture’s data on the GPU is in an undefined state.

- Swift
- Objective-C

```
// Simultaneously modify and synchronize the managed texture's data with the CPU.
let region = MTLRegionMake2D(textureOrigin.x, textureOrigin.y, textureSize.width, textureSize.height)
let bytesPerRow = pixelSize * textureSize.width
imageTexture.replace(region: region, mipmapLevel: 0, withBytes: textureData, bytesPerRow: bytesPerRow)
```

```
// Simultaneously modify and synchronize the managed texture's data with the CPU.
[_imageTexture replaceRegion:MTLRegionMake2D(textureOrigin.x, textureOrigin.y, textureSize.width, textureSize.height)
                 mipmapLevel:0
                   withBytes:textureData
                 bytesPerRow:pixelSize*textureSize.width];
```

After encoding a GPU modification, encode a synchronize(resource:) command. This command updates the entire texture and keeps it synchronized. To update a specific texture slice or mipmap level, encode the synchronize(texture:slice:level:) command instead. Before executing this command, the modified texture’s data on the CPU is in an undefined state.

- Swift
- Objective-C

```
// Create a command buffer for GPU work.
if let commandBuffer = commandQueue.makeCommandBuffer() {
    // Create a compute command encoder.
    guard let computeCommandEncoder =
            commandBuffer.makeComputeCommandEncoder(dispatchType: MTLDispatchType.serial)
    else { return }

    // Encode a compute pass to modify the managed texture's data with the GPU.
    computeCommandEncoder.setComputePipelineState(computePipelineStateObject)
    computeCommandEncoder.setTexture(imageTexture, index: 0)
    computeCommandEncoder.dispatchThreads(gridSize, threadsPerThreadgroup: threadgroupSize)
    computeCommandEncoder.endEncoding()

    // Synchronize the managed texture.
    guard let blitCommandEncoder = commandBuffer.makeBlitCommandEncoder() else { return }
    blitCommandEncoder.synchronize(resource: imageTexture)
    blitCommandEncoder.endEncoding()

    // Add a completion handler.
    commandBuffer.addCompletedHandler { commandBuffer in
        // Once the completion handler is called, it's safe to use the managed resource on CPU.
    }

    // Commit the command buffer.
    commandBuffer.commit()
}
```

```
// Create a command buffer for GPU work.
id  commandBuffer = [_commandQueue commandBuffer];

// Encode a compute pass to modify the managed texture's data with the GPU.
id  computeCommandEncoder = [commandBuffer computeCommandEncoderWithDispatchType:MTLDispatchTypeSerial];
[computeCommandEncoder setComputePipelineState:computePipelineStateObject];
[computeCommandEncoder setTexture:_imageTexture
                          atIndex:0];
[computeCommandEncoder dispatchThreads:gridSize
                 threadsPerThreadgroup:threadgroupSize];
[computeCommandEncoder endEncoding];

// Synchronize the managed texture with an ecoded command.
id  blitCommandEncoder = [commandBuffer blitCommandEncoder];
[blitCommandEncoder synchronizeResource:_imageTexture];
[blitCommandEncoder endEncoding];

// Add a completion handler and commit the command buffer.
[commandBuffer addCompletedHandler:^(id commandBuffer) {
    // Once the completion handler is called, it's safe to use the managed resource on CPU.
}];
[commandBuffer commit];
```

## See Also

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

Choosing a Resource Storage Mode for Intel and AMD GPUs

Select an appropriate storage mode for your textures and buffers on AMD and Intel GPUs.

Copying Data to a Private Resource

Use a blit command encoder to copy buffer or texture data to a private resource.

Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

Reducing the Memory Footprint of Metal Apps

Learn best practices for using memory efficiently in iOS and tvOS.

