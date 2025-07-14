

- Metal
-  MTLSharedEvent 

Protocol

# MTLSharedEvent

An object you use to synchronize access to Metal resources across multiple CPUs, GPUs, and processes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
protocol MTLSharedEvent : MTLEvent
```

## Mentioned in 

About Synchronization Events

Synchronizing Events Across Multiple Devices or Processes

## Overview

The MTLSharedEvent protocol inherits from and adds additional behaviors to MTLEvent. Use shared events only when you need to synchronize changes to resources across multiple Metal device objects, across processes, or between a device object and CPU access to resources. Otherwise, use nonshared events.

Don’t implement this protocol yourself; instead, to create a MTLSharedEvent object, call the makeSharedEvent() method of a MTLDevice object.

To pass this event to another process, first create a handle to the shared event by calling its makeSharedEventHandle() method. Then, transfer the handle to another process with XPC, and from that process, call the makeSharedEvent(handle:) of a MTLDevice object.

For more information, see Synchronizing Events Across Multiple Devices or Processes and Synchronizing Events Between a GPU and the CPU.

## Topics

### Synchronizing a Shareable Event

var signaledValue: UInt64

The current signal value for the shareable event.

**Required**

func notify(MTLSharedEventListener, atValue: UInt64, block: MTLSharedEventNotificationBlock)

Schedules a notification handler to be called after the shareable event’s signal value equals or exceeds a given value.

**Required**

### Creating a Shared Event Handle

func makeSharedEventHandle() -> MTLSharedEventHandle

Creates a new shareable event handle.

**Required**

### Instance Methods

func wait(untilSignaledValue: UInt64, timeoutMS: UInt64) -> Bool

**Required**

## Relationships

### Inherits From

- MTLEvent
- NSObjectProtocol

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

protocol MTLEvent

A simple semaphore to synchronize access to Metal resources.

class MTLSharedEventHandle

An object you use to recreate a shareable event.

class MTLSharedEventListener

A listener for shareable event notifications.

typealias MTLSharedEventNotificationBlock

A block of code invoked after a shareable event’s signal value equals or exceeds a given value.

