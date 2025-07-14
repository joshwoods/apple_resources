

- Metal
- Buffers
-  Tracking the Resource Residency of Argument Buffers 

Article

# Tracking the Resource Residency of Argument Buffers

Optimize resource performance within an argument buffer.

## Overview

The Metal driver can’t automatically track the residency of argument buffer resources, but you can track it manually.

### Track Argument Buffer Resource Residency Manually

Call an MTLRenderCommandEncoder or MTLComputeCommandEncoder method:

- For individual resources, call useResource(_:usage:stages:) or useResource(_:usage:).

- For all resources in a heap, call useHeap(_:stages:) or useHeap(_:).

These methods perform two important functions:

- They add argument buffer resources to the set of resources that the render or compute pass needs resident.

- They ensure that argument buffer resources are in a format that’s compatible with the required function operation, as an MTLResourceUsage value specifies.

The methods with a `stages` parameter also insert dependency hazards, similar to MTLFence instances for that stage.

Call these methods before issuing any draw or dispatch calls that may access the specified resources.

Note

To track resource access and dependency hazards, use MTLFence instances.

If all the required resources aren’t resident when executing a render or compute pass, the associated MTLCommandBuffer instance fails.

## See Also

### Argument Buffers

Improving CPU Performance by Using Argument Buffers

Optimize your app’s performance by grouping your resources into argument buffers.

Managing groups of resources with argument buffers

Create argument buffers to organize related resources.

Indexing Argument Buffers

Assign resource indices within an argument buffer.

Rendering Terrain Dynamically with Argument Buffers

Use argument buffers to render terrain in real time with a GPU-driven pipeline.

Encoding Argument Buffers on the GPU

Use a compute pass to encode an argument buffer and access its arguments in a subsequent render pass.

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

class MTLArgumentDescriptor

A representation of an argument within an argument buffer.

protocol MTLArgumentEncoder

An object used to encode data into an argument buffer.

let MTLAttributeStrideStatic: Int

