

- Virtualization
-  VZVirtioEntropyDeviceConfiguration 

Class

# VZVirtioEntropyDeviceConfiguration

A source of entropy for the guest’s random number generator.

macOS 11.0+

``` source
class VZVirtioEntropyDeviceConfiguration
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

## Overview

Use a VZVirtioEntropyDeviceConfiguration object to expose a source of entropy for the guest operating system’s random-number generator. When you create this object and add it to your virtual machine’s configuration, the virtual machine configures a Virtio-compliant entropy device. The guest operating system uses this device as a seed to generate random numbers.

Create a VZVirtioEntropyDeviceConfiguration object and add it to the entropyDevices property of your virtual machine’s configuration.

## Topics

### Creating the configuration object

init()

Creates an entropy device configuration object.

## Relationships

### Inherits From

- VZEntropyDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZEntropyDeviceConfiguration

The common configuration traits for entropy devices.

