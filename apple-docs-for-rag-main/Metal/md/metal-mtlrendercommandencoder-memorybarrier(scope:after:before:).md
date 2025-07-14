

- Metal
- MTLRenderCommandEncoder
-  memoryBarrier(scope:after:before:) 

Instance Method

# memoryBarrier(scope:after:before:)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func memoryBarrier(
    scope: MTLBarrierScope,
    after: MTLRenderStages,
    before: MTLRenderStages
)
```

**Required**

## Parameters 

`scope`  

An MTLBarrierScope instance that represents the resource types the barrier synchronizes operations on.

`after`  

The render stages of previous draw commands that modify resources of the types that `scope` defines.

`before`  

The render stages of subsequent draw commands that read or modify resources of the types that `scope` defines.

## Discussion

Memory barriers ensure the relevant stages of prior draw commands finish updating resources before starting the stages of subsequent commands that depend on those resources.

To determine whether a GPU supports memory barriers, see the Metal feature set tables (PDF).

## See Also

### Encoding Resource Synchronization Commands

func waitForFence(any MTLFence, before: MTLRenderStages)

Encodes a command that instructs the GPU to pause before starting one or more stages of the render pass until a pass updates a fence.

**Required**

func updateFence(any MTLFence, after: MTLRenderStages)

Encodes a command that instructs the GPU to update a fence after one or more stages, which signals passes waiting on the fence.

**Required**

func memoryBarrier(resources: [any MTLResource], after: MTLRenderStages, before: MTLRenderStages)

Creates a memory barrier that enforces the order of write and read operations for specific resources.

