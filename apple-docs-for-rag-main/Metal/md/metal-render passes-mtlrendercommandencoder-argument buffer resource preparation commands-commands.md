

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Argument Buffer Resource Preparation Commands 

API Collection

# Argument Buffer Resource Preparation Commands

Load individual resources and multiple resources within a heap into GPU memory so that they’re available to shaders through argument buffers.

## Overview

The commands these methods encode ensure your shaders can access resources through one or more argument buffers by loading them into GPU memory. To load an individual resource, call useResource(_:usage:stages:), or another resource-based method. Alternatively, you can load all the resources within a heap by calling useHeap(_:stages:) or another heap-based method.

Important

The heap-based methods don’t provide a `usage` parameter (see MTLResourceUsage) and set the usage for the resources within each heap to read.

To give shaders write or read/write access to specific resources within a heap, call a resource-based method after the heap-based method. Metal combines usage modes set for a resource through both heap and resource methods.

For more information, see Improving CPU Performance by Using Argument Buffers.

## Topics

### Loading Individual Resources for Argument Buffers

func useResource(any MTLResource, usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to a resource.

**Required**

func useResources([any MTLResource], usage: MTLResourceUsage, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to multiple resources.

### Loading Heaps and the Resources They Contain for Argument Buffers

func useHeap(any MTLHeap, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from a heap.

**Required**

func useHeaps([any MTLHeap], stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

## See Also

### Encoding Resource Preparation Commands

Mesh and Object Shader Resource Preparation Commands

Assign resources to mesh and object shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Vertex Shader Resource Preparation Commands

Assign resources to vertex shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Fragment Shader Resource Preparation Commands

Assign resources to fragment shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Tile Shaders Resource Preparation Commands

Assign resources to tile shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

