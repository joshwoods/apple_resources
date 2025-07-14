

- Metal
- MTLRenderCommandEncoder
-  useResource(\_:usage:stages:) 

Instance Method

# useResource(\_:usage:stages:)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func useResource(
    _ resource: any MTLResource,
    usage: MTLResourceUsage,
    stages: MTLRenderStages
)
```

**Required**

## Parameters 

`resource`  

An MTLResource instance that subsequent draw commands depend on.

`usage`  

All the applicable access types the render pass’s shaders use for the resource, including read and write.

For applicable resources, you may be able to prevent the GPU from unnecessarily decompressing color attachments on some devices by setting `usage` to read.

`stages`  

All the render stages that depend on `resource`, including object, mesh, vertex, fragment, and tile.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

Tracking the Resource Residency of Argument Buffers

## Discussion

You can make a resource *resident* (available in GPU memory) for the remaining duration of the render pass by calling this method. Call the method before encoding draw calls that may access `resource` through an argument buffer. The method ensures the resource is in a format that’s compatible with the shaders that depend on it.

Note

You don’t need to call this method if you bind a resource to a shader stage.

For example, you can explicitly bind resources for the vertex stage with the methods in the Vertex Shader Resource Preparation Commands collection.

The method also informs Metal when to apply hazard tracking for a resource you create with MTLHazardTrackingMode.tracked. For a resource you create with MTLHazardTrackingMode.untracked, you need to apply an MTLFence or an MTLEvent to account for potential reading and writing hazards.

You can reconfigure an individual resource’s `usage` options for subsequent draw calls in the same render pass by calling this method again.

Apps typically call the method for a resource in an argument buffer as a part of their *bindless* implementation. For more information about argument buffers and bindless implementations, see Improving CPU Performance by Using Argument Buffers and Go bindless with Metal 3, respectively.

## See Also

### Loading Individual Resources for Argument Buffers

func useResources([any MTLResource], usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to multiple resources.

