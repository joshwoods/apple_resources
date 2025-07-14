

- DeviceDiscoveryExtension
- DDDeviceEvent
-  init(eventType:device:) 

Initializer

# init(eventType:device:)

Creates an event object that conveys status for a discovered device of interest.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
init(
    eventType type: DDDeviceEvent.EventType,
    device: DDDevice
)
```

## Parameters 

`type`  

The option that represents the device’s status in the device discovery life cycle.

`device`  

The discovered device of interest.

