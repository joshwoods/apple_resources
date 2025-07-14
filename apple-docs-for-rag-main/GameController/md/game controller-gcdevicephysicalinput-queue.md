

- Game Controller
- GCDevicePhysicalInput
-  queue 

Instance Property

# queue

The dispatch queue that the system uses for callbacks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var queue: dispatch_queue_t? { get set }
```

**Required**

## Mentioned in 

Handling input events

## Discussion

Objects that conform to the GCDevicePhysicalInput protocol dispatch callbacks on the device’s handlerQueue property by default. If you want to use a different dispatch queue, set this property to the preferred queue before you set callbacks.

