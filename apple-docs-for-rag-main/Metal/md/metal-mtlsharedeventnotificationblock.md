

- Metal
-  MTLSharedEventNotificationBlock 

Type Alias

# MTLSharedEventNotificationBlock

A block of code invoked after a shareable event’s signal value equals or exceeds a given value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLSharedEventNotificationBlock = (any MTLSharedEvent, UInt64) -> Void
```

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

class MTLSharedEventHandle

An object you use to recreate a shareable event.

class MTLSharedEventListener

A listener for shareable event notifications.

