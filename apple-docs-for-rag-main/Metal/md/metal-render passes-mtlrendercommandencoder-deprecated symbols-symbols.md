

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

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

func textureBarrier()

Adds a barrier, which forces any texture read operations to wait until write operations to the same texture finish.

**Required**

Deprecated

