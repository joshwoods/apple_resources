

- Metal
- MTLComputeCommandEncoder
-  updateFence(\_:) 

Instance Method

# updateFence(\_:)

Encodes a command that instructs the GPU to update a fence, allowing passes waiting on the fence to start or resume.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func updateFence(_ fence: any MTLFence)
```

**Required**

## Parameters 

`fence`  

An MTLFence instance to update.

## Discussion

Fences maintain command buffer order to prevent GPU data hazards as the GPU runs various passes. The GPU driver evaluates fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

Important

For a compute pass that updates and waits for the same fence, call waitForFence(_:) before you call updateFence(_:). Updating a fence before waiting on it in the same encoder can cause a GPU deadlock.

On Apple family GPUs, MTLComputeCommandEncoder instances place all fence update commands at the end of their pass.

## See Also

### Synchronizing Across Command Execution

func waitForFence(any MTLFence)

Encodes a command that instructs the GPU to pause pass execution until a fence updates.

**Required**

func memoryBarrier(scope: MTLBarrierScope)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

**Required**

func memoryBarrier(resources: [any MTLResource])

Creates a memory barrier that enforces the order of write and read operations for specific resources.

