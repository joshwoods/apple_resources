

- Metal
- MTLComputeCommandEncoder
-  useHeap(\_:) 

Instance Method

# useHeap(\_:)

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from a heap.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func useHeap(_ heap: any MTLHeap)
```

**Required**

## Parameters 

`heap`  

An MTLHeap instance containing resources used in an argument buffer.

## Mentioned in 

Tracking the Resource Residency of Argument Buffers

Simplifying GPU Resource Management with Residency Sets

## Discussion

You can make the resources in `heap` *resident* (available in GPU memory) for the remaining duration of the render pass by calling this method. Call the method before encoding draw calls that may access resources within `heap` through an argument buffer. The method ensures each resource is in a format that’s compatible with the shaders that depend on it.

This method applies the read resource usage option to all of the resources within the `heaps`, except for textures. The method ignores any texture that has renderTarget, shaderWrite, or both in its usage property. For all other textures in each of the `heaps`, the method optimizes each texture’s memory layout for rendering with a sampler. However, your kernels can’t read from those textures by calling this method because the texture needs a different memory layout that’s suitable for reading.

Important

You can instruct Metal to allow a kernel to read from a texture or write to resources in the heaps by calling useResource(_:usage:).

Methods that apply a usage option for resources (see Encoding Resident Resources) override any previous calls that apply to a resource. For example, you can change the usage option of any heap in `heaps` to write by passing it to useResource(_:usage:stages:) after calling this method. However, you can’t reverse the call order because this method resets the usage for all resources within `heap` to read, overriding previous calls to useResource(_:usage:).

This method instructs Metal to apply hazard tracking for resources you allocate from a heap that you create with MTLHazardTrackingMode.tracked. However, for untracked resources — which come from heaps you create with MTLHazardTrackingMode.untracked — you need to account for hazards by applying MTLFence or MTLEvent instances.

Note

The hazardTrackingMode property of a new MTLHeapDescriptor instance is MTLHazardTrackingMode.default, which is equivalent to MTLHazardTrackingMode.untracked because heaps don’t track resources by default.

Apps typically call the method for heaps that have resources in argument buffers for a *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Encoding Resident Resources

func useResource(any MTLResource, usage: MTLResourceUsage)

Ensures kernel calls that the system encodes in subsequent commands have access to a resource.

**Required**

func useResources([any MTLResource], usage: MTLResourceUsage)

Ensures kernel calls that the system encodes in subsequent commands have access to multiple resources.

func useHeaps([any MTLHeap])

Ensures the shaders in the render pass’s subsequent draw commands have access to all of the resources you allocate from multiple heaps.

