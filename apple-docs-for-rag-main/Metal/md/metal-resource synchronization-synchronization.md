

- Metal
-  Resource Synchronization 

API Collection

# Resource Synchronization

Coordinate the contents of data buffers, textures, and other resources that CPUs and GPUs share access to.

## Overview

By default, Metal tracks the write hazards and synchronizes the resources (see Resource Fundamentals) you create from an MTLDevice and directly bind to a pipeline. However, Metal doesn’t, by default, track resources you allocate from an MTLHeap (see Memory Heaps).

Note

You can also create a resource from a Metal device and set it to MTLHazardTrackingMode.untracked, or create a resource from a Metal heap and set it to MTLHazardTrackingMode.tracked.

Your app is responsible for manually synchronizing the resources that Metal doesn’t track. You can synchronize resources with these mechanisms, which are in ascending scope order:

- Memory barriers

- Memory fences

- Metal events

- Metal shared events

A memory barrier forces any subsequent commands to wait until the previous commands in a pass (such as a render or compute pass) finishes using memory. You can limit the scope of a memory barrier to a buffer, texture, render attachment, or a combination.

An MTLFence synchronizes access to one or more resources across different passes within a command buffer. Use fences to specify any inter-pass resource dependencies within the same command buffer.

An MTLEvent synchronizes access to one or more resources on a single MTLDevice. You can tell the GPU to pause work until another command signals an event. See Synchronizing Events Within a Single Device for more information.

An MTLSharedEvent synchronizes access to one or more resources with other Metal device instances or with the CPU. Shared events are similar to a regular event, but with a larger scope that goes beyond a single GPU to include the CPU and other GPUs. See Synchronizing Events Between a GPU and the CPU and Synchronizing Events Across Multiple Devices or Processes for more information.

Tip

For better performance, use the synchronization mechanism with the smallest scope possible.

## Topics

### Synchronization

Use semaphores or events to coordinate actions across threads to avoid multi-threaded resource contention by copying shared data to multiple buffers.

Synchronizing CPU and GPU Work

Avoid stalls between CPU and GPU work by using multiple instances of a resource.

struct MTLRenderStages

The stages in a render pass that triggers a synchronization command.

### Memory Barriers and Fences

Memory barriers and fences synchronize resource data within a command buffer.

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

struct MTLBarrierScope

Describes the types of resources that a barrier operates on.

protocol MTLFence

A memory fence to capture, track, and manage resource dependencies across command encoders.

### Signal Events

Events synchronize resource data across multiple command buffers, GPU devices, or processes.

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

About Synchronization Events

Synchronize access to resources in your app by signaling events.

Synchronizing Events Within a Single Device

Use nonshareable events to synchronize your app’s work within a single device.

Synchronizing Events Across Multiple Devices or Processes

Use shareable events to synchronize your app’s work across multiple devices or processes.

Synchronizing Events Between a GPU and the CPU

Use shareable events to synchronize your app’s work between a GPU and the CPU.

protocol MTLEvent

A simple semaphore to synchronize access to Metal resources.

protocol MTLSharedEvent

An object you use to synchronize access to Metal resources across multiple CPUs, GPUs, and processes.

class MTLSharedEventHandle

An object you use to recreate a shareable event.

class MTLSharedEventListener

A listener for shareable event notifications.

typealias MTLSharedEventNotificationBlock

A block of code invoked after a shareable event’s signal value equals or exceeds a given value.

## See Also

### Resources

Resource Fundamentals

Learn the common attributes of all Metal memory resources, including buffers and textures, and how to manage the underlying memory.

Buffers

Create and manage untyped data your app uses to exchange information with its shader functions.

Textures

Create and manage typed data your app uses to exchange information with its shader functions.

Memory Heaps

Take control of your app’s GPU memory management by creating a large memory allocation for various buffers, textures, and other resources.

Resource Loading

Load assets in your games and apps quickly by running a dedicated input/output queue alongside your GPU tasks.

