

- Metal
- MTLComputeCommandEncoder
-  useResource(\_:usage:) 

Instance Method

# useResource(\_:usage:)

Ensures kernel calls that the system encodes in subsequent commands have access to a resource.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func useResource(
    _ resource: any MTLResource,
    usage: MTLResourceUsage
)
```

**Required**

## Parameters 

`resource`  

An MTLResource instance used in an argument buffer.

`usage`  

How the compute pass can access data, including read and write permission.

For applicable resources, you may be able to prevent the GPU from unnecessarily decompressing color attachments on some devices by setting `usage` to read.

## Mentioned in 

Tracking the Resource Residency of Argument Buffers

Simplifying GPU Resource Management with Residency Sets

## Discussion

You can make a resource *resident* (available in GPU memory) for the remaining duration of the compute pass by calling this method. Call the method before encoding function calls that may access the `resource` through an argument buffer. The method ensures the resource is in a format that’s compatible with the kernels that depend on it.

Note

You don’t need to call this method if you bind a resource for compute kernels to access.

The method also informs Metal when to apply hazard tracking for a resource you create with MTLHazardTrackingMode.tracked. For a resource you create with MTLHazardTrackingMode.untracked, you need to apply an MTLFence or an MTLEvent to account for potential reading and writing hazards.

You can reconfigure an individual resource’s `usage` options for subsequent draw calls in the same render pass by calling this method again.

Apps typically call this method for a resource in an argument buffer as a part of their *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Encoding Resident Resources

func useResources([any MTLResource], usage: MTLResourceUsage)

Ensures kernel calls that the system encodes in subsequent commands have access to multiple resources.

func useHeap(any MTLHeap)

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from a heap.

**Required**

func useHeaps([any MTLHeap])

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from multiple heaps.

