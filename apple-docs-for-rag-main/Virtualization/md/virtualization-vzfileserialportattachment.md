

- Virtualization
-  VZFileSerialPortAttachment 

Class

# VZFileSerialPortAttachment

An attachment point that writes data from the guest system to a file.

macOS 11.0+

``` source
class VZFileSerialPortAttachment
```

## Overview

Use a VZFileSerialPortAttachment object to configure a one-way serial port from the guest operating system to the virtual machine. When the guest sends data to the serial port, the virtual machine writes that data to the specified file. You can’t use this serial port to send data back to the guest.

Create a VZSerialPortAttachment object and assign it to an appropriate subclass of VZSerialPortConfiguration object, such as VZVirtioConsoleDeviceConfiguration. The file you use to create this object must be writable.

## Topics

### Creating the attachment point

init(url: URL, append: Bool) throws

Creates a file-based serial port attachment object.

### Getting the file details

var url: URL

The URL of a file on the local file system.

var append: Bool

A Boolean that indicates whether the virtual machine appends data to the file.

## Relationships

### Inherits From

- VZSerialPortAttachment

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

class VZSerialPortAttachment

The common behaviors for the serial attachment points of your virtual machine.

