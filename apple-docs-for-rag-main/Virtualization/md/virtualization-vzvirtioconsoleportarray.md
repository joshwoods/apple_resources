

- Virtualization
-  VZVirtioConsolePortArray 

Class

# VZVirtioConsolePortArray

A class that represents a collection of Virtio console ports.

macOS 13.0+

``` source
class VZVirtioConsolePortArray
```

## Topics

### Determining the number of ports

var maximumPortCount: UInt32

An unsigned integer that represents the maximum number of ports allocated by this device.

### Accessing a specific port

subscript(Int) -> VZVirtioConsolePort?

Returns the Virtio console port at the specified index.

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

### Related Documentation

class VZVirtioConsoleDevice

A class that represents a Virtio console device in a virtual machine.

### Console ports

class VZVirtioConsolePort

A class that represents a Virtio console port in a VM.

