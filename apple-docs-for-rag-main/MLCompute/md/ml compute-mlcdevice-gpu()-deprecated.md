

- ML Compute
- MLCDevice
-  gpu() Deprecated

Type Method

# gpu()

Creates a device that uses a GPU, if one exists.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func gpu() -> Self?
```

## Return Value

A device that uses a GPU, or `nil` if no GPU exists.

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

class func ane() -> Self?

Creates a device that uses the Apple Neural Engine, if one exists.

Deprecated

