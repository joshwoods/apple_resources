

- ML Compute
- MLCDevice
-  cpu() Deprecated

Type Method

# cpu()

Creates a device that uses the CPU.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func cpu() -> Self
```

## Return Value

A device that uses the CPU.

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

class func gpu() -> Self?

Creates a device that uses a GPU, if one exists.

Deprecated

class func ane() -> Self?

Creates a device that uses the Apple Neural Engine, if one exists.

Deprecated

