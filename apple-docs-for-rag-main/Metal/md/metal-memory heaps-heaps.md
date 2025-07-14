

- Metal
-  Memory Heaps 

API Collection

# Memory Heaps

Take control of your app’s GPU memory management by creating a large memory allocation for various buffers, textures, and other resources.

## Overview

Use an MTLHeap to quickly create and destroy GPU resources. Heaps can also help your apps save memory by aliasing portions of it in multiple places.

Create a heap by calling an MTLDevice instance’s makeHeap(descriptor:) method.

Note

Metal only synchronizes resources that you create from a Metal heap and that have the hazardTrackingMode property set to MTLHazardTrackingMode.tracked.

## Topics

### Resource Memory Allocation and Management

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

protocol MTLHeap

A memory pool from which you can suballocate resources.

class MTLHeapDescriptor

A configuration that customizes the behavior for a Metal memory heap.

enum MTLHeapType

The options you use to choose the heap type.

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

## See Also

### Resources

Resource Fundamentals

Learn the common attributes of all Metal memory resources, including buffers and textures, and how to manage the underlying memory.

Buffers

Create and manage untyped data your app uses to exchange information with its shader functions.

Textures

Create and manage typed data your app uses to exchange information with its shader functions.

Resource Loading

Load assets in your games and apps quickly by running a dedicated input/output queue alongside your GPU tasks.

Resource Synchronization

Coordinate the contents of data buffers, textures, and other resources that CPUs and GPUs share access to.

