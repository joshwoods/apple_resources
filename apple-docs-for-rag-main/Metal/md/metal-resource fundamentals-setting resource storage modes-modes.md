

- Metal
- Resource Fundamentals
-  Setting Resource Storage Modes 

Article

# Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

## Overview

Storage modes are only set when creating an instance, and the system default allows for access to memory from both the CPU and GPU. Metal selects the default mode for resources depending on hardware.

- For Apple silicon GPUs the default is MTLStorageMode.shared.

- For Intel-based Mac computers, the default is MTLStorageMode.managed for all MTLTexture instances and MTLBuffer instances attached to discrete GPUs. MTLBuffer instances using the integrated GPU have MTLStorageMode.shared as their default.

Important

Use the system default if your data is available to both the CPU and GPU. When you manually select shared or managed mode, your app may not run on some hardware.

You perform the same synchronization tasks to ensure GPU and CPU memory coherency in both default modes. To check for GPU architecture and capabilities, use the supportsFamily(_:) method instead of the storageMode property. See Detecting GPU Features and Metal Software Versions for more information.

Use MTLStorageMode.memoryless, only available on Apple silicon, when you manage your own storage, or want to run a GPU task that requires temporary resources. For tasks that share memory on the GPU, use MTLStorageMode.private storage. This article includes examples of how to set the storage mode for a buffer or texture.

For more guidance on which mode to choose, see Choosing a Resource Storage Mode for Apple GPUs and Choosing a Resource Storage Mode for Intel and AMD GPUs.

### Set a Storage Mode for a Buffer

Create a new MTLBuffer with the makeBuffer(length:options:) method and set its storage mode in the method’s `options` parameter.

- Swift
- Objective-C

```
let bufferOptions = MTLResourceOptions.storageModePrivate
let buffer = device.makeBuffer(length: 256,
                               options: bufferOptions)
```

```
MTLResourceOptions bufferOptions = MTLResourceStorageModePrivate;
id  buffer = [_device newBufferWithLength:256
                                             options:bufferOptions];
```

Note

The storage mode options in MTLResourceOptions are equivalent to the storage mode values in MTLStorageMode. When you create a new buffer, you can combine multiple resource options but you can set only one storage mode.

### Set a Storage Mode for a Texture

Create a new MTLTextureDescriptor and set its storage mode in the descriptor’s storageMode property. Then create a new MTLTexture with the makeTexture(descriptor:) method.

- Swift
- Objective-C

```
let textureDescriptor = MTLTextureDescriptor.texture2DDescriptor(pixelFormat: .bgra8Unorm,
                                                                 width: 256,
                                                                 height: 256,
                                                                 mipmapped: true)
textureDescriptor.storageMode = .private
let texture = device.makeTexture(descriptor: textureDescriptor)
```

```
MTLTextureDescriptor *textureDescriptor = [MTLTextureDescriptor texture2DDescriptorWithPixelFormat:MTLPixelFormatBGRA8Unorm
                                                                                             width:256
                                                                                            height:256
                                                                                         mipmapped:YES];
textureDescriptor.storageMode = MTLStorageModePrivate;
id  texture = [_device newTextureWithDescriptor:textureDescriptor];
```

## See Also

### Resource Management

Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

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

