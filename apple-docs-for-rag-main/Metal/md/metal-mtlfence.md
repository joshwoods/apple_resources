

- Metal
-  MTLFence 

Protocol

# MTLFence

A memory fence to capture, track, and manage resource dependencies across command encoders.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
protocol MTLFence : NSObjectProtocol
```

## Mentioned in 

Tracking the Resource Residency of Argument Buffers

## Overview

An MTLFence instance is typically used to track a resource created from an MTLHeap instance. You can also track non-heap resources that have tracking mode hazardTrackingModeUntracked.

To create an MTLFence instance, call the makeFence() method of an MTLDevice instance. A command encoder can either update a fence or wait for a fence.

Tip

When using a fence across multiple MTLCommandQueue instances, commit the queue that updates a fence before committing the queue that waits on a fence. Consider using an MTLEvent instead of a fence for these situations.

| Command encoders | Methods that update a fence | Methods that wait for a fence |
|----|----|----|
| MTLBlitCommandEncoder | updateFence(_:) | waitForFence(_:) |
| MTLComputeCommandEncoder | updateFence(_:) | waitForFence(_:) |
| MTLRenderCommandEncoder | updateFence(_:after:) | waitForFence(_:before:) |
| MTLAccelerationStructureCommandEncoder | updateFence(_:) | waitForFence(_:) |
| MTLResourceStateCommandEncoder | update(_:) | wait(for:) |

## Topics

### Identifying the Fence

var device: any MTLDevice

The device object that created the fence.

**Required**

var label: String?

A string that identifies the fence.

**Required**

### Specifying Render Stages

struct MTLRenderStages

The stages in a render pass that triggers a synchronization command.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Memory Barriers and Fences

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

struct MTLBarrierScope

Describes the types of resources that a barrier operates on.

