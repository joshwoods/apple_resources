

- Metal
- Resource Fundamentals
-  Choosing a Resource Storage Mode for Apple GPUs 

Article

# Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

## Overview

Apple GPUs have a unified memory model in which the CPU and the GPU share system memory. However, CPU and GPU access to that memory depends on the storage mode you choose for your resources. The MTLStorageMode.shared mode defines system memory that both the CPU and the GPU can access. The MTLStorageMode.private mode defines system memory that only the GPU can access.

The MTLStorageMode.memoryless mode defines tile memory within the GPU that only the GPU can access. Tile memory has higher bandwidth, lower latency, and consumes less power than system memory.

### Choose a Resource Storage Mode for Buffers or Textures

The storage mode you choose depends on how you plan to use Metal resources:

Populate and update on the CPU  
Data shared by the CPU and GPU. Use MTLStorageMode.shared. The CPU and GPU share data. This is the default for buffer and texture storage.

Access exclusively on the GPU  
Data owned by the GPU. Use MTLStorageMode.private. Choose the mode if you populate your resource with the GPU through a compute, render, or blit pass. This case is common for render targets, intermediary resources, or texture streaming. For guidance on how to copy data to a private resource, see Copying Data to a Private Resource.

Populate on CPU and access frequently on GPU  
Shared integrated memory for the CPU and GPU. Use MTLStorageMode.shared.

Temporary texture contents for GPU passes  
Memory held by the GPU for textures within or between passes. Use MTLStorageMode.memoryless. Memoryless mode only works for textures, and stores temporary resources in tiled memory for high performance. An example is a depth or stencil texture thatʼs used only within a single pass and isnʼt needed in an earlier or later rendering stage.

For information on setting storage modes in your app, see Setting Resource Storage Modes.

### Create a Memoryless Render Target

To create a memoryless render target, set the storageMode property of an MTLTextureDescriptor to MTLStorageMode.memoryless and use this descriptor to create a new MTLTexture. Then set this new texture as the texture property of an MTLRenderPassAttachmentDescriptor.

- Swift
- Objective-C

```
let memorylessDescriptor = MTLTextureDescriptor.texture2DDescriptor(pixelFormat: .r16Float,
                                                                    width: 256,
                                                                    height: 256,
                                                                    mipmapped: true)
memorylessDescriptor.storageMode = .memoryless
let memorylessTexture = device.makeTexture(descriptor: memorylessDescriptor)

let renderPassDescriptor = MTLRenderPassDescriptor()
renderPassDescriptor.depthAttachment.texture = memorylessTexture
```

```
MTLTextureDescriptor *memorylessDescriptor = [MTLTextureDescriptor texture2DDescriptorWithPixelFormat:MTLPixelFormatR16Float
                                                                                                width:256
                                                                                               height:256
                                                                                            mipmapped:YES];
memorylessDescriptor.storageMode = MTLStorageModeMemoryless;
id  memorylessTexture = [_device newTextureWithDescriptor:memorylessDescriptor];

MTLRenderPassDescriptor *renderPassDescriptor = [MTLRenderPassDescriptor renderPassDescriptor];
renderPassDescriptor.depthAttachment.texture = memorylessTexture;
```

See Rendering a Scene with Deferred Lighting in Objective-C for an example of an app that uses a memoryless render target.

Note

You can create only textures, not buffers, using MTLStorageMode.memoryless mode. You can’t use buffers as memoryless render targets.

## See Also

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

Choosing a Resource Storage Mode for Intel and AMD GPUs

Select an appropriate storage mode for your textures and buffers on AMD and Intel GPUs.

Copying Data to a Private Resource

Use a blit command encoder to copy buffer or texture data to a private resource.

Synchronizing a Managed Resource in macOS

Manually synchronize memory for a Metal resource in apps.

Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

Reducing the Memory Footprint of Metal Apps

Learn best practices for using memory efficiently in iOS and tvOS.

