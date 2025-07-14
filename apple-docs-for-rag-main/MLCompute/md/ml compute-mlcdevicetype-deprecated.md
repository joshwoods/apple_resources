

- ML Compute
-  MLCDeviceType Deprecated

Enumeration

# MLCDeviceType

A device type for execution of a neural network.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCDeviceType
```

## Topics

### Device Types

case any

A device type that represents either the CPU or GPU.

case cpu

A device type that represents the CPU.

case gpu

A device type that represents the GPU.

case ane

A device type that represents the Apple Neural Engine.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Devices

convenience init?(type: MLCDeviceType)

Creates a device of the type you specify.

Deprecated

convenience init?(type: MLCDeviceType, selectsMultipleComputeDevices: Bool)

Creates a device that you can configure to use multiple compute devices.

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

