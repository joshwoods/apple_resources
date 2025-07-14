

- Metal
- Resource Synchronization
-  Synchronizing Events Within a Single Device 

Article

# Synchronizing Events Within a Single Device

Use nonshareable events to synchronize your app’s work within a single device.

## Overview

The following figure and code show a nonshareable event that synchronizes graphics rendering on one command queue with compute processing on another.

- Swift
- Objective-C

```
func setupSingleDeviceEvent() {
    // Nonshareable event
    event = device.makeEvent()

    // Command queues
    commandQueueA = device.makeCommandQueue()
    commandQueueB = device.makeCommandQueue()
}

func renderFrame() {
    guard
        let event = event,
        let commandBufferA = commandQueueA?.makeCommandBuffer(),
        let commandBufferB = commandQueueB?.makeCommandBuffer()
        else { return }

    // Command Queue A (Graphics Rendering)
    /* Encode first render pass */
    commandBufferA.encodeSignalEvent(event, value: 1)
    /* Encode second render pass */
    commandBufferA.encodeWaitForEvent(event, value: 2)
    /* Encode third render pass */
    commandBufferA.commit()

    // Command Queue B (Compute Processing)
    /* Encode first compute pass */
    commandBufferB.encodeWaitForEvent(event, value: 1)
    /* Encode second compute pass */
    commandBufferB.encodeSignalEvent(event, value: 2)
    /* Encode third compute pass */
    commandBufferB.commit()
}
```

```
- (void)setupSingleDeviceEvent
{
    // Nonshareable event
    _event = [_device newEvent];

    // Command queues
    _commandQueueA = [_device newCommandQueue];
    _commandQueueB = [_device newCommandQueue];
}

- (void)renderFrame
{
    // Command Queue A (Graphics Rendering)
    id commandBufferA = [_commandQueueA commandBuffer];
    /* Encode first render pass */
    [commandBufferA encodeSignalEvent:_event value:1];
    /* Encode second render pass */
    [commandBufferA encodeWaitForEvent:_event value:2];
    /* Encode third render pass */
    [commandBufferA commit];

    // Command Queue B (Compute Processing)
    id commandBufferB = [_commandQueueB commandBuffer];
    /* Encode first compute pass */
    [commandBufferB encodeWaitForEvent:_event value:1];
    /* Encode second compute pass */
    [commandBufferB encodeSignalEvent:_event value:2];
    /* Encode third compute pass */
    [commandBufferB commit];
}
```

During setup, the code creates a nonshareable event and two command queues. Then, to render a frame, the code encodes render commands onto the first queue and compute commands on the second queue. While the code shows these commands being encoded sequentially, in a real app, you should determine whether you can encode the commands for each command queue on a different thread.

The first render pass and first compute pass are assumed to not depend on each other’s results and modify the same data. By encoding them on different queues, the device object can schedule these commands concurrently.

When two sets of commands have dependencies on each other, the code expresses these dependencies by signaling or waiting on the event. When each queue reaches a command that waits for an event, that queue blocks further execution until the event is signaled.

## See Also

### Signal Events

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

About Synchronization Events

Synchronize access to resources in your app by signaling events.

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

