

- ML Compute
- MLCDevice
-  init(gpuDevices:) Deprecated

Initializer

# init(gpuDevices:)

Creates a device using the GPUs you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(gpuDevices gpus: [any MTLDevice])
```

## Parameters 

`gpus`  

An array that contains specific Metal devices you’ll use to execute neural networks.

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

class func cpu() -> Self

Creates a device that uses the CPU.

Deprecated

class func gpu() -> Self?

Creates a device that uses a GPU, if one exists.

Deprecated

class func ane() -> Self?

Creates a device that uses the Apple Neural Engine, if one exists.

Deprecated

