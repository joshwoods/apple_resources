

- Metal
- Resource Fundamentals
-  Choosing a Resource Storage Mode for Intel and AMD GPUs 

Article

# Choosing a Resource Storage Mode for Intel and AMD GPUs

Select an appropriate storage mode for your textures and buffers on AMD and Intel GPUs.

## Overview

A Mac can have multiple GPUs, each with a unified or discrete memory model. In a *unified memory model*, the CPU and the GPU share system memory. However, CPU and GPU access to that memory depends on the storage mode you choose for your resources. In a *discrete memory model*, system memory is separate from video memory. System memory is accessible to both the CPU and the GPU, but video memory is accessible only to the GPU.

The Metal framework’s resource storage mode API works for both unified and discrete memory models, so you don’t need to write specific code for either.

### Understand the Different Metal Memory Modes

In both memory models, a resource with an MTLStorageMode.shared mode resides in system memory accessible to both the CPU and the GPU. Shared resources are only available on systems with integrated graphics, such as Apple silicon and integrated GPUs on Intel-based Mac computers.

A resource with an MTLStorageMode.private mode is accessible only to the GPU. In a unified memory model, this resource resides in system memory. In a discrete memory model, it resides in video memory. In both memory models, Metal optimizes GPU access to private resources.

In a discrete memory model, Metal always attempts to store private resources in video memory. However, under certain memory constraints, Metal may evict a private resource into system memory. When you use a private resource that Metal previously evicted, Metal attempts to copy it back into video memory before you use it.

In a unified memory model, a resource with an MTLStorageMode.managed mode resides in system memory accessible to both the CPU and the GPU.

In a discrete memory model, a managed resource exists as a synchronized pair of memory allocations. One copy of the resource resides in system memory accessible only to the CPU; the other resides in video memory accessible only to the GPU. However, you don’t manage the copies separately; Metal creates a single MTLResource instance to access both.

In both memory models, Metal optimizes CPU and GPU access to managed resources. However, you must explicitly synchronize a managed resource after modifying its contents with the CPU or the GPU. For information about synchronizing a managed resource, see Synchronizing a Managed Resource in macOS.

### Choose a Storage Mode for Resources

Your storage mode should depend on the resource type and how your application uses storage accessed by Metal. Understanding the underlying memory architecture gives context and helps you investigate where you can optimize storage and synchronization. On Intel-based Mac computers, follow these guidelines:

- Prefer the default storage mode selected by Metal. Metal selects the optimal mode for the resource type and hardware.

- Use the MTLStorageMode.private mode when creating a resource that’s only accessed by the GPU. This includes temporary targets for render passes.

- To optimize for workloads initialized from CPU and then only processed on GPU, copy from a CPU-populated resource in the default storage mode to a GPU-only MTLResource with MTLStorageMode.private storage. See Copying Data to a Private Resource for details.

You’re responsible for signaling synchronization between the CPU and GPU with managed and shared storage. Regardless of your resource size, try and keep your synchronization points as light and infrequent as possible. Batch GPU work together to help reduce frequent synchronization. See Synchronizing a Managed Resource in macOS for details.

To detect the GPU architecture and features at runtime, use the supportsFamily(_:) method. See Detecting GPU Features and Metal Software Versions for more information, and the Metal feature set tables (PDF) for full information on hardware support in Apple devices and computers.

## See Also

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

Copying Data to a Private Resource

Use a blit command encoder to copy buffer or texture data to a private resource.

Synchronizing a Managed Resource in macOS

Manually synchronize memory for a Metal resource in apps.

Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

Reducing the Memory Footprint of Metal Apps

Learn best practices for using memory efficiently in iOS and tvOS.

