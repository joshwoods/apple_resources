

- Virtualization
-  VZFileHandleSerialPortAttachment 

Class

# VZFileHandleSerialPortAttachment

An attachment point that allows bidirectional communication using file handles.

macOS 11.0+

``` source
class VZFileHandleSerialPortAttachment
```

## Overview

Use a VZFileHandleSerialPortAttachment object to configure a serial port using separate file handles for reading and writing data. In your virtual machine, use the file handles in this object in the following way:

- To send data to the guest operating system, write data to the file handle in the fileHandleForReading property.

- To receive data from the guest operating system, read data from the file handle in the fileHandleForWriting property.

## Topics

### Creating the attachment point

init(fileHandleForReading: FileHandle?, fileHandleForWriting: FileHandle?)

Creates a serial port attachment object from the specified file handles.

### Getting the file handles

var fileHandleForReading: FileHandle?

The file handle that the guest operating system uses to read data.

var fileHandleForWriting: FileHandle?

The file handle that the guest operating system uses to write data.

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

class VZFileSerialPortAttachment

An attachment point that writes data from the guest system to a file.

class VZSerialPortAttachment

The common behaviors for the serial attachment points of your virtual machine.

