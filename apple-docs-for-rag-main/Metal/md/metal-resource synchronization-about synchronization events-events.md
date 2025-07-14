

- Metal
- Resource Synchronization
-  About Synchronization Events 

Article

# About Synchronization Events

Synchronize access to resources in your app by signaling events.

## Overview

Use events to specify synchronization points in your app. For example, you might use an event to synchronize graphics rendering commands running on one command queue with compute processing being performed on another command queue.

Metal provides two different kinds of events:

- Nonshareable. MTLEvent objects synchronize events within a single device object.

- Shareable. MTLSharedEvent objects synchronize events across multiple device objects, processors, or processes.

Shareable events have a higher overhead than nonshareable events. Don’t use MTLSharedEvent to synchronize events within a single device object; use MTLEvent instead.

### Event Signaling and Waiting

An event contains a monotonically increasing unsigned 64-bit integer. An event starts with a value of `0`. You can either update the event’s value by *signaling* it, or block further execution by *waiting* on the event. Typically, you keep an integer value in your app for each event and increase its value each time you need to synchronize on the event. For example, you might increment the number each time you render a new frame of animation.

To signal a change to the event, call encodeSignalEvent(_:value:) on a command buffer, passing in the new value for this event. Metal signals the event after all scheduled commands prior to the event have finished, updating the event’s value if the new value is larger than its current value.

To wait for an event to be signaled, call encodeWaitForEvent(_:value:) on a command buffer, passing in the value to wait for. Commands that are after this event on the queue are not executed until the event’s value is at least as large as the value you provide.

Note

You can only encode events outside command encoder boundaries, not between encoded commands of a command encoder.

## See Also

### Signal Events

Implementing a Multistage Image Filter Using Heaps and Events

Use events to synchronize access to resources allocated on a heap.

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

