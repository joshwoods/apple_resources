

- Virtualization
-  VZSerialPortConfiguration 

Class

# VZSerialPortConfiguration

The common configuration traits for serial port requests.

macOS 11.0+

``` source
class VZSerialPortConfiguration
```

## Overview

Don’t create a VZSerialPortConfiguration object directly. Instead, instantiate a concrete instance of one of its subclasses, such as VZVirtioConsoleDeviceConfiguration. Use the attachment property of this class to configure the medium through which serial communication happens.

## Topics

### Configuring the Attachment Point

var attachment: VZSerialPortAttachment?

The object that defines how the configuration of the virtual machine’s serial port interfaces.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioConsoleDeviceSerialPortConfiguration

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

class VZVirtioConsoleDeviceSerialPortConfiguration

A configuration object that requests the creation of a console device to communicate with the guest system.

