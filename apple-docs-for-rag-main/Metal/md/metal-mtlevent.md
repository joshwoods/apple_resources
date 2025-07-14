

- Metal
-  MTLEvent 

Protocol

# MTLEvent

A simple semaphore to synchronize access to Metal resources.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
protocol MTLEvent : NSObjectProtocol
```

## Mentioned in 

About Synchronization Events

## Overview

You can only get an MTLEvent using the makeEvent() method of an MTLDevice instance. Events allow you to synchronize commands executing on a single Metal device.

An event is an unsigned 64-bit integer, starting with an initial value of `0` and can only increase in value afterwards. You signal an event change by calling an MTLCommandBuffer instance’s encodeSignalEvent(_:value:) method. The command buffer signals the event after the GPU completes running all previous commands, and updates its value if necessary.

To wait for an event signal, call encodeWaitForEvent(_:value:) on a command buffer, passing in the value to wait for. When the device executes the command buffer and reaches this wait command, it compares the event’s current value to the provided value. The device only starts new commands when the event reaches a value equal to or greater than the requested value.

You can encode signaling and waiting on events into different command buffers, even command buffers executing on two different command queues for the same device. You can also encode these commands independently of each other, meaning, for example, that you can wait on signals you haven’t encoded yet.

For more information, see Synchronizing Events Within a Single Device.

## Topics

### Identifying the Event

var device: (any MTLDevice)?

The device object that created the event.

**Required**

var label: String?

A string that identifies the event.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTLSharedEvent

## See Also

### Signal Events

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

protocol MTLSharedEvent

An object you use to synchronize access to Metal resources across multiple CPUs, GPUs, and processes.

class MTLSharedEventHandle

An object you use to recreate a shareable event.

class MTLSharedEventListener

A listener for shareable event notifications.

typealias MTLSharedEventNotificationBlock

A block of code invoked after a shareable event’s signal value equals or exceeds a given value.

