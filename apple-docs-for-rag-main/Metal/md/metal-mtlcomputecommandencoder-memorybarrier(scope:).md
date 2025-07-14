

- Metal
- MTLComputeCommandEncoder
-  memoryBarrier(scope:) 

Instance Method

# memoryBarrier(scope:)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func memoryBarrier(scope: MTLBarrierScope)
```

**Required**

## Parameters 

`scope`  

An MTLBarrierScope instance that represents the resource types the barrier synchronizes operations on.

## Discussion

Memory barriers ensure the relevant passes finish updating resources before starting the stages of subsequent commands that depend on those resources.

To determine whether a GPU supports memory barriers, see the Metal feature set tables (PDF).

## See Also

### Synchronizing Across Command Execution

func waitForFence(any MTLFence)

Encodes a command that instructs the GPU to pause pass execution until a fence updates.

**Required**

func updateFence(any MTLFence)

Encodes a command that instructs the GPU to update a fence, allowing passes waiting on the fence to start or resume.

**Required**

func memoryBarrier(resources: [any MTLResource])

Creates a memory barrier that enforces the order of write and read operations for specific resources.

