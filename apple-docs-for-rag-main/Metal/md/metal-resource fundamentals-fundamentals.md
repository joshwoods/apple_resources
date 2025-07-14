

- Metal
-  Resource Fundamentals 

API Collection

# Resource Fundamentals

Learn the common attributes of all Metal memory resources, including buffers and textures, and how to manage the underlying memory.

## Overview

A *resource* is a memory asset, such as an MTLBuffer or MTLTexture, that a GPU can access (see Buffers and Textures).

You can either allocate a resource from an MTLDevice instance or an MTLHeap instance (see Memory Heaps). Metal sets a resource’s hazardTrackingMode property to MTLHazardTrackingMode.default if you don’t specify another tracking mode. The default value depends on what Metal instance creates the resource.

- Resources from Metal device instances default to MTLHazardTrackingMode.tracked.

- Resources from Metal heap instances default to MTLHazardTrackingMode.untracked.

Each resource your app creates typically uses one of these storage modes:

MTLStorageMode.private  
Apps can only access resources in private storage from the GPU.

MTLStorageMode.shared  
Apps can access resources in shared storage from both the CPU and the GPU.

MTLStorageMode.managed  
Apps can access resources in managed storage from both the CPU and the GPU, just like shared storage. However, the GPU backs resources in managed mode with memory in private storage.

Private mode resources give your app optimization opportunities that shared mode resources don’t. Managed mode resources also give your app the same opportunities and allow your to app access them from the CPU.

## Topics

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

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

### Residency Sets

Simplifying GPU Resource Management with Residency Sets

Organize your resources into groups and influence when they become accessible to the GPU.

protocol MTLResidencySet

A collection of resource allocations that can move in and out of resident memory.

class MTLResidencySetDescriptor

A configuration that customizes the behavior for a residency set.

### Common Resource Functionality

protocol MTLAllocation

A memory allocation from a Metal GPU device, such as a memory heap, texture, or data buffer.

protocol MTLResource

An allocation of memory accessible to a GPU.

struct MTLResourceOptions

Optional arguments used to set the behavior of a resource.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

struct MTLResourceID

## See Also

### Resources

Buffers

Create and manage untyped data your app uses to exchange information with its shader functions.

Textures

Create and manage typed data your app uses to exchange information with its shader functions.

Memory Heaps

Take control of your app’s GPU memory management by creating a large memory allocation for various buffers, textures, and other resources.

Resource Loading

Load assets in your games and apps quickly by running a dedicated input/output queue alongside your GPU tasks.

Resource Synchronization

Coordinate the contents of data buffers, textures, and other resources that CPUs and GPUs share access to.

