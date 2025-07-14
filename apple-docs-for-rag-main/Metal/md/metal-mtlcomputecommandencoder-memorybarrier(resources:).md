

- Metal
- MTLComputeCommandEncoder
-  memoryBarrier(resources:) 

Instance Method

# memoryBarrier(resources:)

Creates a memory barrier that enforces the order of write and read operations for specific resources.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func memoryBarrier(resources: [any MTLResource])
```

## Parameters 

`resources`  

An array of MTLResource instances the barrier applies to.

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

func memoryBarrier(scope: MTLBarrierScope)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

**Required**

