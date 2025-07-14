

- Virtualization
-  VZVirtioConsoleDeviceSerialPortConfiguration 

Class

# VZVirtioConsoleDeviceSerialPortConfiguration

A configuration object that requests the creation of a console device to communicate with the guest system.

macOS 11.0+

``` source
class VZVirtioConsoleDeviceSerialPortConfiguration
```

## Overview

A VZVirtioConsoleDeviceSerialPortConfiguration object enables serial communication between the guest operating system and host computer through the Virtio interface. After you create this configuration object, configure its inherited attachment property with an object that defines the type of serial communication you want to enable. Use a VZFileHandleSerialPortAttachment object to enable two-way communication between the guest and host, and use a VZFileSerialPortAttachment object to enable one-way communication from the guest to the file you designate.

## Topics

### Creating the Configuration Object

init()

Creates a serial port configuration object.

## Relationships

### Inherits From

- VZSerialPortConfiguration

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

class VZSerialPortConfiguration

The common configuration traits for serial port requests.

