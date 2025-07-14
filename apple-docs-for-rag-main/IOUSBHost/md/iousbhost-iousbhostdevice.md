

- IOUSBHost
-  IOUSBHostDevice 

Class

# IOUSBHostDevice

The class that claims and configures devices, retrieves descriptors, and sends device requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostDevice
```

## Overview

This class enables management of the device state, including sending control requests to the default endpoint 0, configuring the device, and resetting the device. The interest handler also allows monitoring of the device state. The client creates the class and initializes it with initWithIOService:options:queue:error:interestHandler:.

Note

To prevent other drivers from changing the state of your device, maintain an IOUSBHostDevice object until you no longer need control over the device.

## Topics

### Retrieving Device Descriptors

var configurationDescriptor: UnsafePointer&lt;IOUSBConfigurationDescriptor>?

The currently selected configuration descriptor.

### Resetting the Device

func reset() throws

Terminates the device and attempts to re-enumerate it.

## Relationships

### Inherits From

- IOUSBHostObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

