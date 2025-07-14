

- DeviceDiscoveryExtension
- DDDiscoveryExtension
-  didReceiveEvent(\_:) 

Instance Method

# didReceiveEvent(\_:)

Provides a device event from the system to the extension.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOSvisionOS

``` source
func didReceiveEvent(_ event: DDDeviceEvent)
```

**Required** Default implementation provided.

## Parameters 

`event`  

A moment of interest in the device discovery life cycle.

## Discussion

The system calls this function to give the app’s `DDDiscoveryExtension` information about the device. For example, when someone selects the device in the AirPlay menu (AVRoutePickerView), the system notifies the extension of the state change by invoking this callback.

## Default Implementations

### DDDiscoveryExtension Implementations

func didReceiveEvent(DDDeviceEvent)

A default, blank implementation for when the system notifies the extension of a device event.

