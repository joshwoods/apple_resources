

- ML Compute
- MLCDevice
-  init(type:selectsMultipleComputeDevices:) Deprecated

Initializer

# init(type:selectsMultipleComputeDevices:)

Creates a device that you can configure to use multiple compute devices.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
convenience init?(
    type: MLCDeviceType,
    selectsMultipleComputeDevices: Bool
)
```

## Parameters 

`type`  

The device type.

`selectsMultipleComputeDevices`  

A Boolean that indicates whether to select multiple compute devices if the system supports it.

## Discussion

For the `type` parameter, use MLCDeviceType.any unless you need to control device selection. This ensures that the framework selects the best device to execute the neural network.

## See Also

### Creating Devices

convenience init?(type: MLCDeviceType)

Creates a device of the type you specify.

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

class func ane() -> Self?

Creates a device that uses the Apple Neural Engine, if one exists.

Deprecated

