

- Metal
- MTLRenderCommandEncoder
-  use(\_:count:stages:) Deprecated

Instance Method

# use(\_:count:stages:)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS

``` source
func use(
    _ heaps: UnsafePointer,
    count: Int,
    stages: MTLRenderStages
)
```

Deprecated

Call useHeaps(_:stages:) instead.

## Parameters 

`heaps`  

A pointer to a C array of MTLHeap instances with resources that subsequent draw commands depend on.

`count`  

The number of elements in `heaps`.

`stages`  

All the render stages that depend on resources within `heaps`, including object, mesh, vertex, fragment, and tile.

## Discussion

You can make the resources in `heaps` *resident* (available in GPU memory) for the remaining duration of the render pass by calling this method. Call the method before encoding draw calls that may access resources within `heaps` through an argument buffer. The method ensures each resource is in a format that’s compatible with the shaders that depend on it.

The method’s applies the read resource usage option to all of the resources within `heaps`, except for textures. The method ignores any texture that has renderTarget, shaderWrite, or both in its usage property. For all other textures in `heaps`, the method optimizes each texture’s memory layout for rendering with a sampler. However, your shaders can’t read from those textures by calling this method because the texture needs a different memory layout that’s suitable for reading.

Important

You can instruct Metal to allow a shader to read from texture or write to other resources in heap, by calling useResource(_:usage:stages:).

Methods that apply a usage option for resources (see Argument Buffer Resource Preparation Commands) override any previous calls that apply to a resource. For example, you can change the usage option for a buffer to write by passing it to useResource(_:usage:stages:) after calling this method. However, you can’t reverse the call order because this method resets the usage for all resources within `heaps` to read, overriding previous calls to useResource(_:usage:stages:).

The method instructs Metal to apply hazard tracking for resources you allocate from a heap that you create with MTLHazardTrackingMode.tracked. However, for untracked resources — which come from heaps you create with MTLHazardTrackingMode.untracked — you need to account for hazards by applying MTLFence or MTLEvent instances.

Note

The hazardTrackingMode property of a new MTLHeapDescriptor instance is MTLHazardTrackingMode.default, which is equivalent to MTLHazardTrackingMode.untracked because heaps don’t track resources by default.

Apps typically call the method for heaps that have resources in argument buffers for a *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Deprecated Methods

func useResource(any MTLResource, usage: MTLResourceUsage)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

**Required**

Deprecated

func use(any MTLResource, usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

Deprecated

func useResources([any MTLResource], usage: MTLResourceUsage)

Ensures the shaders in the render pass’s subsequent draw commands have access to multiple resources.

Deprecated

func use(UnsafePointer&lt;any MTLResource>, count: Int, usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to multiple resources.

Deprecated

func useHeap(any MTLHeap)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from a heap.

**Required**

Deprecated

func use(any MTLHeap, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from a heap.

Deprecated

func useHeaps([any MTLHeap])

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

Deprecated

func textureBarrier()

Adds a barrier, which forces any texture read operations to wait until write operations to the same texture finish.

**Required**

Deprecated

