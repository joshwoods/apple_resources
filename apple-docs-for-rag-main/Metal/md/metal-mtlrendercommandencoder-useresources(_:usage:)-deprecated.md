

- Metal
- MTLRenderCommandEncoder
-  useResources(\_:usage:) Deprecated

Instance Method

# useResources(\_:usage:)

Ensures the shaders in the render pass’s subsequent draw commands have access to multiple resources.

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac CatalystmacOS 10.13–13.0DeprecatedtvOS 11.0–16.0DeprecatedvisionOS

``` source
func useResources(
    _ resources: [any MTLResource],
    usage: MTLResourceUsage
)
```

Deprecated

Call useResources(_:usage:stages:) instead.

## Parameters 

`resources`  

An array of MTLResource instances that subsequent draw commands depend on.

`usage`  

All the applicable access types the render pass’s shaders use for `resources`, including read and write.

For applicable resources, you may be able to prevent the GPU from unnecessarily decompressing color attachments on some devices by setting `usage` to read.

## Discussion

You can make a resource *resident* (available in GPU memory) for the remaining duration of the render pass by calling this method. Call the method before encoding draw calls that may access `resource` through an argument buffer. The method ensures the resource is in a format that’s compatible with the shaders that depend on it.

Note

You don’t need to call this method if you bind a resource to a shader stage.

For example, you can explicitly bind resources for the vertex stage with the methods in the Vertex Shader Resource Preparation Commands collection.

The method also informs Metal when to apply hazard tracking for a resource you create with MTLHazardTrackingMode.tracked. For a resource you create with MTLHazardTrackingMode.untracked, you need to apply an MTLFence or an MTLEvent to account for potential reading and writing hazards.

You can reconfigure an individual resource’s `usage` options for subsequent draw calls in the same render pass by calling this method again.

Apps typically call the method for a resource in an argument buffer as a part of their *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Deprecated Methods

func useResource(any MTLResource, usage: MTLResourceUsage)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

**Required**

Deprecated

func use(any MTLResource, usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

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

func use(UnsafePointer&lt;any MTLHeap>, count: Int, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

Deprecated

func textureBarrier()

Adds a barrier, which forces any texture read operations to wait until write operations to the same texture finish.

**Required**

Deprecated

