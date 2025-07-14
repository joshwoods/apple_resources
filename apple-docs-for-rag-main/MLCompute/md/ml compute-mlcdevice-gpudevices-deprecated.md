

- ML Compute
- MLCDevice
-  gpuDevices Deprecated

Instance Property

# gpuDevices

An array that contains the specific Metal devices you use to execute neural networks.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var gpuDevices: [any MTLDevice] { get }
```

## See Also

### Inspecting Devices

var type: MLCDeviceType

The type you specify when creating the device.

Deprecated

var actualDeviceType: MLCDeviceType

The active device.

Deprecated

