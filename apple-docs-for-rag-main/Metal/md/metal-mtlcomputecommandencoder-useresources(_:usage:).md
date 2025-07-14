

- Metal
- MTLComputeCommandEncoder
-  useResources(\_:usage:) 

Instance Method

# useResources(\_:usage:)

Ensures kernel calls that the system encodes in subsequent commands have access to multiple resources.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func useResources(
    _ resources: [any MTLResource],
    usage: MTLResourceUsage
)
```

## Parameters 

`resources`  

A list of MTLResource instances used in one or more argument buffers.

`usage`  

All the applicable access types for use of these resources, including read and write. Your resource usage type applies to all resources passed to this method call.

For applicable resources, you may be able to prevent the GPU from unnecessarily decompressing color attachments on some devices by setting `usage` to read.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

You can make many resources *resident* (available in GPU memory) for the remaining duration of the compute pass by calling this method. Call the method before encoding function calls that may access these `resources` through an argument buffer. The method ensures the resource is in a format that’s compatible with the kernels that depend on it.

Note

You don’t need to call this method if you bind a resource for compute kernels to access.

The method also informs Metal when to apply hazard tracking for a resource you create with MTLHazardTrackingMode.tracked. For a resource you create with MTLHazardTrackingMode.untracked, you need to apply an MTLFence or an MTLEvent to account for potential reading and writing hazards.

You can reconfigure an individual resource’s `usage` options for subsequent draw calls with the useResource(_:usage:) method.

Apps typically call this method for a resource in an argument buffer as a part of their *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Encoding Resident Resources

func useResource(any MTLResource, usage: MTLResourceUsage)

Ensures kernel calls that the system encodes in subsequent commands have access to a resource.

**Required**

func useHeap(any MTLHeap)

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from a heap.

**Required**

func useHeaps([any MTLHeap])

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from multiple heaps.

