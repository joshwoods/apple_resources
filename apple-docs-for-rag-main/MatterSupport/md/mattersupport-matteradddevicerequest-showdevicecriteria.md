

- MatterSupport
- MatterAddDeviceRequest
-  showDeviceCriteria 

Instance Property

# showDeviceCriteria

A predicate that filters what devices appear in the picker.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
var showDeviceCriteria: MatterAddDeviceRequest.DeviceCriteria
```

## Discussion

During setup user interface flows, the system may present a picker to choose the device to set up. Only devices that match the specified criteria appear in the picker.

Use `.allDevices` to display all devices. Use `.not(...)` to hide blocked devices, such as those already paired in the ecosystem.

## See Also

### Defining the device criteria

enum DeviceCriteria

A predicate to match against possible devices that may appear in the picker.

