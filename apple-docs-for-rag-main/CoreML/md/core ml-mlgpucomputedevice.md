

- Core ML
-  MLGPUComputeDevice 

Class

# MLGPUComputeDevice

An object that represents a GPU compute device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class MLGPUComputeDevice
```

## Topics

### Getting The Metal Device

var metalDevice: (any MTLDevice)!

The device that represents the underlying metal device.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MLComputeDeviceProtocol
- NSObjectProtocol
- Sendable

## See Also

### Compute devices

enum MLComputeDevice

Compute devices for framework operations.

class MLCPUComputeDevice

An object that represents a CPU compute device.

class MLNeuralEngineComputeDevice

An object that represents a Neural Engine compute device.

protocol MLComputeDeviceProtocol

An interface that represents a compute device type.

