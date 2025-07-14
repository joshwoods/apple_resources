

- Virtualization
-  VZSpiceAgentPortAttachment 

Class

# VZSpiceAgentPortAttachment

An attachment point that enables the Spice clipboard sharing capability.

macOS 13.0+

``` source
class VZSpiceAgentPortAttachment
```

## Topics

### Creating a shared clipboard

init()

Creates a new Spice agent port attachment.

### Enabling clipboard sharing between the host and the VM

var sharesClipboard: Bool

A Boolean value that indicates whether the framework needs to share the clipboard between the host and the VM.

### Naming the Virtio console port for the Spice guest agent

class var spiceAgentPortName: String

The name of the Virtio console port for the Spice guest agent.

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

