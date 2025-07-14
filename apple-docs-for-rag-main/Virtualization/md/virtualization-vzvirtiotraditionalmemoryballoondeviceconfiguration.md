

- Virtualization
-  VZVirtioTraditionalMemoryBalloonDeviceConfiguration 

Class

# VZVirtioTraditionalMemoryBalloonDeviceConfiguration

A configuration object that provides a way to reclaim memory from the guest system.

macOS 11.0+

``` source
class VZVirtioTraditionalMemoryBalloonDeviceConfiguration
```

## Overview

Create a `VZVirtioTraditionalMemoryBalloonDeviceConfiguration` object when you want the ability to reclaim memory from the guest operating system. After creating this object, add it to the memoryBalloonDevices property of your VZVirtualMachineConfiguration object. In response, the virtual machine provides a VZVirtioTraditionalMemoryBalloonDevice object, which you use to initiate memory-related requests with the guest system. Access that object from the memoryBalloonDevices property of VZVirtualMachine.

Important

Create only one `VZVirtioTraditionalMemoryBalloonDeviceConfiguration` object for your virtual machine.

## Topics

### Creating the Configuration Object

init()

Creates a memory ballon device configuration object to include with your virtual machine’s configuration data.

## Relationships

### Inherits From

- VZMemoryBalloonDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuration

class VZMemoryBalloonDeviceConfiguration

The common configuration traits for memory balloon devices.

