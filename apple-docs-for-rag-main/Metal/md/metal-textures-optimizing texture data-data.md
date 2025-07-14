

- Metal
- Textures
-  Optimizing Texture Data 

Article

# Optimizing Texture Data

Optimize a texture’s data to improve GPU or CPU access.

## Overview

By default, Metal attempts to optimize a texture’s data for both GPU or CPU accesses based on the texture’s storage mode and usage options. You can improve a texture’s performance on the GPU or CPU by specifically optimizing the texture’s data for either use case. You can also opt out of optimization altogether. Optimizing a texture’s performance for one use can decrease that texture’s performance for another.

Before optimizing texture data, carefully consider the storage modes and usage options for your textures. For guidance on resource storage modes, see Setting Resource Storage Modes. For guidance on texture usage options, see MTLTextureUsage.

Note

Metal may not be able to optimize some textures for specific hardware and ignores optimization API calls for those textures.

### Optimize Texture Data for GPU Access

By default, Metal attempts to optimize texture data for GPU access if it meets any of these conditions:

- You create the texture with an MTLStorageMode.private mode.

- You create the texture with an renderTarget option.

If the texture doesn’t meet any of these conditions, you can optimize your texture data explicitly. After you create your texture and populate its contents, encode and commit an optimizeContentsForGPUAccess(texture:) or optimizeContentsForGPUAccess(texture:slice:level:) command.

- Swift
- Objective-C

```
// Create the first texture.
let texture1GPUOptimized: MTLTexture! = nil
...

// Put content in the texture.
...

// Create a command buffer to submit work to the GPU.
let commandBuffer: MTLCommandBuffer! = commandQueue.makeCommandBuffer()

// Optimize the texture for GPU access by encoding a blit command.
let blitEncoder: MTLBlitCommandEncoder! = commandBuffer.makeBlitCommandEncoder()
blitEncoder.optimizeContentsForGPUAccess(texture: texture1GPUOptimized)

// End the encoding.
blitEncoder.endEncoding()

// Add a completion handler.
commandBuffer.addCompletedHandler {_ in
    // Texture 1 is optimized for CPU access.
    ...
}

// Commit the command buffer to the command queue.
commandBuffer.commit()
```

```
// Create the first texture.
id  texture1GPUOptimized;
...

// Put content in the texture.
...

// Create a command buffer to submit work to the GPU.
id  commandBuffer = [commandQueue commandBuffer];

// Optimize the texture for GPU access by encoding a blit command.
id  blitEncoder = [commandBuffer blitCommandEncoder];
[blitEncoder optimizeContentsForGPUAccess:texture1GPUOptimized];

// End the encoding.
[blitEncoder endEncoding];

// Add a completion handler.
[commandBuffer addCompletedHandler:^(id cb) {
    // Texture 1 is optimized for CPU access.
    ...
}];

// Commit the command buffer to the command queue.
[commandBuffer commit];
```

To optimize a drawable from an MTKView for GPU access, set the view’s framebufferOnly property to true. This property configures the texture exclusively as a render target and displayable resource.

### Optimize Texture Data for CPU Access

By default, Metal attempts to optimize texture data for CPU access if it meets both of these conditions:

- You create the texture with an MTLStorageMode.shared or MTLStorageMode.managed mode.

- You write to the texture with the replace(region:mipmapLevel:withBytes:bytesPerRow:) or replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) method.

If you don’t meet both of these conditions, you can optimize your texture data explicitly. After you create your texture and populate its contents, encode and commit an optimizeContentsForCPUAccess(texture:) or optimizeContentsForCPUAccess(texture:slice:level:) command.

- Swift
- Objective-C

```
// Create a second texture.
let texture2CPUOptimized: MTLTexture! = nil
...

// Put content in the texture.
...

// Create a command buffer to submit work to the GPU.
let commandBuffer: MTLCommandBuffer! = commandQueue.makeCommandBuffer()

// Optimize the texture for CPU access by encoding a blit command.
let blitEncoder: MTLBlitCommandEncoder! = commandBuffer.makeBlitCommandEncoder()
blitEncoder.optimizeContentsForCPUAccess(texture: texture2CPUOptimized)

// End encoding and commit it to the command buffer with add a completion handler.
blitEncoder.endEncoding()
commandBuffer.addCompletedHandler {_ in
    // Texture 2 is optimized for CPU access.
    ...
}

// Commit the command buffer to the command queue.
commandBuffer.commit()
```

```
// Create a second texture.
id  texture2CPUOptimized;
...

// Put content in the texture.
...

// Create a command buffer to submit work to the GPU.
id  commandBuffer = [commandQueue commandBuffer];

// Optimize the texture for CPU access by encoding a blit command.
id  blitEncoder = [commandBuffer blitCommandEncoder];
[blitEncoder optimizeContentsForCPUAccess:texture2CPUOptimized];

// End encoding and commit it to the command buffer with add a completion handler.
[blitEncoder endEncoding];
[commandBuffer addCompletedHandler:^(id cb) {
    // Texture 2 is optimized for CPU access.
    ...
}];

// Commit the command buffer to the command queue.
[commandBuffer commit];
```

### Apply Lossless Compression to a Texture on Apple GPUs

Lossless compression is a specific form of GPU optimization that Metal can apply to texture data. Lossless compression reduces a texture’s memory size without discarding any of its data. On devices that support MTLGPUFamily.apple5, Metal attempts to apply lossless compression to a texture if it meets all of these conditions:

- You don’t create the texture with a block-compressed pixel format, such as PVRTC, ASTC, or BC.

- You don’t create the texture with an unknown, shaderWrite, or pixelFormatView option.

- You don’t create the texture from a buffer with the makeTexture(descriptor:offset:bytesPerRow:) method.

Additionally, if you meet both of the following conditions, you can optimize your texture data explicitly so Metal can apply lossless compression:

- You create the texture with an MTLStorageMode.shared mode.

- You write to the texture with the replace(region:mipmapLevel:withBytes:bytesPerRow:) or replace(region:mipmapLevel:slice:withBytes:bytesPerRow:bytesPerImage:) method.

For guidance, see Optimize Texture Data for GPU Access.

### Opt out of Texture Data Optimization for GPU Access

In some cases, your texture data may benefit from opting out of optimization for GPU access, for example, when optimization has regressed your app’s performance (particularly for render target read-backs on the CPU).

First, create a texture descriptor and set its allowGPUOptimizedContents property to false.

- Swift
- Objective-C

```
let textureDescriptor = MTLTextureDescriptor.texture2DDescriptor(pixelFormat: .rgba8Unorm,
                                                                 width: 512,
                                                                 height: 512,
                                                                 mipmapped: false)

// Don't allow the the GPU to optimize the texture.
textureDescriptor.allowGPUOptimizedContents = false
```

```
MTLTextureDescriptor *textureDescriptor =
 [MTLTextureDescriptor texture2DDescriptorWithPixelFormat:MTLPixelFormatRGBA8Unorm
                                                    width:512
                                                   height:512
                                                mipmapped:NO];

// Don't allow the the GPU to optimize the texture.
textureDescriptor.allowGPUOptimizedContents = NO;
```

Then, set the texture descriptor’s storageMode property to MTLStorageMode.shared or MTLStorageMode.managed.

- Swift
- Objective-C

```
// Set the texture descriptor's storage mode to shared or managed based on the GPU family.
if device.supportsFamily(.apple1) {
    textureDescriptor.storageMode = .shared
} else {
    textureDescriptor.storageMode = .managed
}
```

```
// Set the texture descriptor's storage mode to shared or managed based on the GPU family.

if ([device supportsFamily:MTLGPUFamilyApple1]) {
    textureDescriptor.storageMode = MTLStorageModeShared;
} else {
    textureDescriptor.storageMode = MTLStorageModeManaged;
}
```

Finally, create a texture from the texture descriptor.

- Swift
- Objective-C

```
// Create a texture using the texture descriptor.
let texture = device.makeTexture(descriptor: textureDescriptor)
```

```
// Create a texture using the texture descriptor.
id  texture = [device newTextureWithDescriptor:textureDescriptor];
```

## See Also

### Texture Basics

Understanding Color-Renderable Pixel Format Sizes

Know the size limits of color render targets in Apple GPUs based on the target’s pixel format.

protocol MTLTexture

A resource that holds formatted image data.

enum MTLTextureCompressionType

class MTLTextureDescriptor

An object that you use to configure new Metal texture objects.

class MTKTextureLoader

An object that creates textures from existing data in common image formats.

class MTLSharedTextureHandle

A texture handle that can be shared across process address space boundaries.

enum MTLPixelFormat

The data formats that describe the organization and characteristics of individual pixels in a texture.

