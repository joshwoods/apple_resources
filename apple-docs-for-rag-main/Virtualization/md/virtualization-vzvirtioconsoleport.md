

- Virtualization
-  VZVirtioConsolePort 

Class

# VZVirtioConsolePort

A class that represents a Virtio console port in a VM.

macOS 13.0+

``` source
class VZVirtioConsolePort
```

## Overview

Don’t instantiate a `VZVirtioConsolePort` directly. You retrieve this object from the VZVirtioConsoleDevice ports property.

## Topics

### Configuring the port

var name: String?

The name of the port.

var attachment: VZSerialPortAttachment?

An array of serial port attachments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Console ports

class VZVirtioConsolePortArray

A class that represents a collection of Virtio console ports.

