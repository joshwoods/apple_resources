

- Virtualization
-  VZUSBMassStorageDevice 

Class

# VZUSBMassStorageDevice

A class that represents a hot-pluggable USB mass storage device.

macOS 15.0+

``` source
class VZUSBMassStorageDevice
```

## Overview

Create this device either by instantiating it directly and passing VZUSBMassStorageDeviceConfiguration to its initializer, or instantiating a `VZUSBMassStorageDeviceConfiguration` in a VZVirtualMachineConfiguration. Direct instantiation creates an object that you can pass to attach(device:completionHandler:). Instantiation through `VZUSBMassStorageDeviceConfiguration` makes the device available in the usbDevices property.

## Topics

### Creating a USB mass storage device

init(configuration: VZUSBMassStorageDeviceConfiguration)

Creates a USB mass storage device with the provided configuration.

## Relationships

### Inherits From

- VZStorageDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- VZUSBDevice

## See Also

### Related Documentation

class VZUSBController

A class that represents a USB controller in a VM.

