

- Virtualization
-  VZSerialPortAttachment 

Class

# VZSerialPortAttachment

The common behaviors for the serial attachment points of your virtual machine.

macOS 11.0+

``` source
class VZSerialPortAttachment
```

## Overview

Don’t create a VZSerialPortAttachment object directly. Instead, instantiate a concrete subclass such as VZFileHandleSerialPortAttachment to configure how the virtual machine’s serial port connects with the host computer.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZFileHandleSerialPortAttachment
- VZFileSerialPortAttachment
- VZSpiceAgentPortAttachment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Attachment points

class VZFileHandleSerialPortAttachment

An attachment point that allows bidirectional communication using file handles.

class VZFileSerialPortAttachment

An attachment point that writes data from the guest system to a file.

