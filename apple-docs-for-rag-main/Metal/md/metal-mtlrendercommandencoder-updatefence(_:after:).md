

- Metal
- MTLRenderCommandEncoder
-  updateFence(\_:after:) 

Instance Method

# updateFence(\_:after:)

Encodes a command that instructs the GPU to update a fence after one or more stages, which signals passes waiting on the fence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func updateFence(
    _ fence: any MTLFence,
    after stages: MTLRenderStages
)
```

**Required**

## Parameters 

`fence`  

An MTLFence instance the render pass updates after the applicable stages to inform the GPU that it can start or resume any passes waiting for `fence`.

`stages`  

An MTLRenderStages instance that designates which stages in the render pass apply to `fence`.

## Discussion

Fences maintain order to prevent GPU data hazards as the GPU runs various passes, including render passes, within the same command queue. The render pass notifies any passes or stages waiting for `fence` (see waitForFence(_:before:)) each time it finishes running a stage in the `stages` parameter.

Important

For a render pass that updates and waits for the same fence, call waitForFence(_:before:) before calling updateFence(_:after:). Updating a fence before waiting on it within the same encoder can cause GPU deadlock.

The GPU driver evaluates the pass’s fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

Apple family GPUs can update and respond to fences on a per-stage basis. That allows those GPUs to run portions of different stages, such as vertex and fragment, at the same time. You can check whether a GPU is in an Apple GPU family with the supportsFamily(_:) method.

## See Also

### Encoding Resource Synchronization Commands

func waitForFence(any MTLFence, before: MTLRenderStages)

Encodes a command that instructs the GPU to pause before starting one or more stages of the render pass until a pass updates a fence.

**Required**

func memoryBarrier(resources: [any MTLResource], after: MTLRenderStages, before: MTLRenderStages)

Creates a memory barrier that enforces the order of write and read operations for specific resources.

func memoryBarrier(scope: MTLBarrierScope, after: MTLRenderStages, before: MTLRenderStages)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

**Required**

