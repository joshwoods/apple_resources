

- Metal
-  MTLSharedEventHandle 

Class

# MTLSharedEventHandle

An object you use to recreate a shareable event.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MTLSharedEventHandle
```

## Overview

To create a `MTLSharedEventHandle` object, call the makeSharedEventHandle() method on a MTLSharedEvent object. Use an XPC conection to pass a `MTLSharedEventHandle` object to another process. To recreate the event, call the makeSharedEvent(handle:) on a MTLDevice object.

## Topics

### Identifying the Shareable Event Handle

var label: String?

A string that identifies the shareable event.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

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

protocol MTLSharedEvent

An object you use to synchronize access to Metal resources across multiple CPUs, GPUs, and processes.

class MTLSharedEventListener

A listener for shareable event notifications.

typealias MTLSharedEventNotificationBlock

A block of code invoked after a shareable event’s signal value equals or exceeds a given value.

