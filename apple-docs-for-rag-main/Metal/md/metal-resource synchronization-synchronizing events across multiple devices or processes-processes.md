

- Metal
- Resource Synchronization
-  Synchronizing Events Across Multiple Devices or Processes 

Article

# Synchronizing Events Across Multiple Devices or Processes

Use shareable events to synchronize your app’s work across multiple devices or processes.

## Overview

The following figure and code show a shareable event that synchronizes graphics rendering on one device with compute processing on another.

- Swift
- Objective-C

```
func setupMultipleDeviceEvent() {
    // Shareable event
    sharedEvent = deviceA.makeSharedEvent()

    // Built-in GPU command queue
    commandQueueA = deviceA.makeCommandQueue()

    // External GPU command queue
    commandQueueB = deviceB.makeCommandQueue()
}

func renderFrame() {
    guard
        let sharedEvent = sharedEvent,
        let commandBufferA = commandQueueA?.makeCommandBuffer(),
        let commandBufferB = commandQueueB?.makeCommandBuffer()
        else { return }

    // Device A (Graphics Rendering)
    /* Encode first render pass */
    commandBufferA.encodeSignalEvent(sharedEvent, value: 1)
    /* Encode second render pass */
    commandBufferA.encodeWaitForEvent(sharedEvent, value: 2)
    /* Encode third render pass */
    commandBufferA.commit()

    // Device B (Compute Processing)
    /* Encode first compute pass */
    commandBufferB.encodeWaitForEvent(sharedEvent, value: 1)
    /* Encode second compute pass  */
    commandBufferB.encodeSignalEvent(sharedEvent, value: 2)
    /* Encode third compute pass */
    commandBufferB.commit()
}
```

```
- (void)setupMultipleDeviceEvent
{
    // Shareable event
    _sharedEvent = [_deviceA newSharedEvent];

    // Built-in GPU command queue
    _commandQueueA = [_deviceA newCommandQueue];

    // External GPU command queue
    _commandQueueB = [_deviceB newCommandQueue];
}

- (void)renderFrame
{
    // Device A (Graphics Rendering)
    id commandBufferA = [_commandQueueA commandBuffer];
    /* Encode first render pass */
    [commandBufferA encodeSignalEvent:_sharedEvent value:1];
    /* Encode second render pass  */
    [commandBufferA encodeWaitForEvent:_sharedEvent value:2];
    /* Encode third render pass  */
    [commandBufferA commit];

    // Device B (Compute Processing)
    id commandBufferB = [_commandQueueB commandBuffer];
    /* Encode first compute pass */
    [commandBufferB encodeWaitForEvent:_sharedEvent value:1];
    /* Encode second compute pass */
    [commandBufferB encodeSignalEvent:_sharedEvent value:2];
    /* Encode third compute pass */
    [commandBufferB commit];
}
```

During setup, the code creates a shareable event (MTLSharedEvent) and command queues on two different devices. Like the example shown in Synchronizing Events Within a Single Device, it encodes render commands onto the first queue and compute commands on the second queue.

You call the same methods when signaling and waiting on shared events as you do when working with events on a single device. The only difference is that the queues are associated with different devices and the event being used to synchronize access is a shared event.

The code shown above assumes you’ve created each resource on both device objects, and each pair of resources share a single allocation of memory. This strategy means that change made by one device object are visible to the other device object. For an example of how to do this, see Selecting Device Objects for Compute Processing.

## See Also

### Signal Events

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

About Synchronization Events

Synchronize access to resources in your app by signaling events.

Synchronizing Events Within a Single Device

Use nonshareable events to synchronize your app’s work within a single device.

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

