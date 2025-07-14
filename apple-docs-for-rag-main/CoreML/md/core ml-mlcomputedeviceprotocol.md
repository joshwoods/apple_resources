

- Core ML
-  MLComputeDeviceProtocol 

Protocol

# MLComputeDeviceProtocol

An interface that represents a compute device type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol MLComputeDeviceProtocol : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MLCPUComputeDevice
- MLGPUComputeDevice
- MLNeuralEngineComputeDevice

## See Also

### Compute devices

enum MLComputeDevice

Compute devices for framework operations.

class MLCPUComputeDevice

An object that represents a CPU compute device.

class MLGPUComputeDevice

An object that represents a GPU compute device.

class MLNeuralEngineComputeDevice

An object that represents a Neural Engine compute device.

