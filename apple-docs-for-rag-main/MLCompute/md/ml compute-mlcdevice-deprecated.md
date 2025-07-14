

- ML Compute
-  MLCDevice Deprecated

Class

# MLCDevice

An object that represents the CPU or one or more GPUs the framework uses to execute a neural network.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCDevice
```

## Topics

### Creating Devices

convenience init?(type: MLCDeviceType)

Creates a device of the type you specify.

convenience init?(type: MLCDeviceType, selectsMultipleComputeDevices: Bool)

Creates a device that you can configure to use multiple compute devices.

enum MLCDeviceType

A device type for execution of a neural network.

convenience init?(gpuDevices: [any MTLDevice])

Creates a device using the GPUs you specify.

class func cpu() -> Self

Creates a device that uses the CPU.

class func gpu() -> Self?

Creates a device that uses a GPU, if one exists.

class func ane() -> Self?

Creates a device that uses the Apple Neural Engine, if one exists.

### Inspecting Devices

var type: MLCDeviceType

The type you specify when creating the device.

var actualDeviceType: MLCDeviceType

The active device.

var gpuDevices: [any MTLDevice]

An array that contains the specific Metal devices you use to execute neural networks.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

