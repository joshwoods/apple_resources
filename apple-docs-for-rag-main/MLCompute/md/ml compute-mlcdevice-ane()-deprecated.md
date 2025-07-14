

- ML Compute
- MLCDevice
-  ane() Deprecated

Type Method

# ane()

Creates a device that uses the Apple Neural Engine, if one exists.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
class func ane() -> Self?
```

## Return Value

A device that uses the Apple Neural Engine, or `nil` if none exists.

## Discussion

When you select this device, the system uses the Apple Neural Engine to execute valid layers. Layers that can’t execute on the Apple Neural Engine run on the `CPU` or `GPU`. The system doesn’t select the Apple Neural Engine if you use MLCDeviceType.any.

This device applies to inference graphs only. It doesn’t work with a training graph or inference graph that shares layers with a training graph.

## See Also

### Creating Devices

convenience init?(type: MLCDeviceType)

Creates a device of the type you specify.

Deprecated

convenience init?(type: MLCDeviceType, selectsMultipleComputeDevices: Bool)

Creates a device that you can configure to use multiple compute devices.

Deprecated

enum MLCDeviceType

A device type for execution of a neural network.

Deprecated

convenience init?(gpuDevices: [any MTLDevice])

Creates a device using the GPUs you specify.

Deprecated

class func cpu() -> Self

Creates a device that uses the CPU.

Deprecated

class func gpu() -> Self?

Creates a device that uses a GPU, if one exists.

Deprecated

