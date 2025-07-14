

- Metal
- MTLRenderCommandEncoder
-  useHeap(\_:stages:) 

Instance Method

# useHeap(\_:stages:)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from a heap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func useHeap(
    _ heap: any MTLHeap,
    stages: MTLRenderStages
)
```

**Required**

## Parameters 

`heap`  

An MTLHeap instance with resources that subsequent draw commands depend on.

`stages`  

All the render stages that depend on resources within `heap`, including object, mesh, vertex, fragment, and tile.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

Tracking the Resource Residency of Argument Buffers

## Discussion

You can make the resources in `heap` *resident* (available in GPU memory) for the remaining duration of the render pass by calling this method. Call the method before encoding draw calls that may access resources within `heap` through an argument buffer. The method ensures each resource is in a format that’s compatible with the shaders that depend on it.

The method’s applies the read resource usage option to all of the resources within `heap`, except for textures. The method ignores any texture that has renderTarget, shaderWrite, or both in its usage property. For all other textures in `heap`, the method optimizes each texture’s memory layout for rendering with a sampler. However, your shaders can’t read from those textures by calling this method because the texture needs a different memory layout that’s suitable for reading.

Important

You can instruct Metal to allow a shader to read from texture or write to other resources in heap, by calling useResource(_:usage:stages:).

Methods that apply a usage option for resources (see Argument Buffer Resource Preparation Commands) override any previous calls that apply to a resource. For example, you can change the usage option for buffer in `heap` to write by passing it to useResource(_:usage:stages:) after calling this method. However, you can’t reverse the call order because this method resets the usage for all resources within `heap` to read, overriding previous calls to useResource(_:usage:stages:).

The method instructs Metal to apply hazard tracking for resources you allocate from a heap that you create with MTLHazardTrackingMode.tracked. However, for untracked resources — which come from heaps you create with MTLHazardTrackingMode.untracked — you need to account for hazards by applying MTLFence or MTLEvent instances.

Note

The hazardTrackingMode property of a new MTLHeapDescriptor instance is MTLHazardTrackingMode.default, which is equivalent to MTLHazardTrackingMode.untracked because heaps don’t track resources by default.

Apps typically call the method for heaps that have resources in argument buffers for a *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Loading Heaps and the Resources They Contain for Argument Buffers

func useHeaps([any MTLHeap], stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

