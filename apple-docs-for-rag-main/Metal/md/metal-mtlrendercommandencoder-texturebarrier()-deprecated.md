

- Metal
- MTLRenderCommandEncoder
-  textureBarrier() Deprecated

Instance Method

# textureBarrier()

Adds a barrier, which forces any texture read operations to wait until write operations to the same texture finish.

macOS 10.11–10.14Deprecated

``` source
func textureBarrier()
```

**Required**

Deprecated

Call memoryBarrier(scope:after:before:) instead.

## Discussion

Use a barrier if you use the same texture for both an input to a shader and as a rendering destination for the render pass.

A barrier let’s your app safely write to and then correctly read from the same texture. The barrier ensures that the draw calls before the barrier finish their write operations before any draw calls after the barrier read from the texture.

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

func use(UnsafePointer&lt;any MTLHeap>, count: Int, stages: MTLRenderStages)

Ensures the shaders in the render pass’s subsequent draw commands have access to the resources you allocate from multiple heaps.

Deprecated

