

- Virtualization
-  VZMacKeyboardConfiguration 

Class

# VZMacKeyboardConfiguration

A device that defines the configuration for a Mac keyboard.

macOS 14.0+

``` source
class VZMacKeyboardConfiguration
```

## Overview

Use this configuration to attach a Mac keyboard configuration to a VM. A VZVirtualMachineView can use this device to send key events to the VM, including the Mac-specific key events, such as the Globe key.

## Topics

### Creating a new Mac keyboard configuration

init()

Creates a new Mac keyboard configuration.

## Relationships

### Inherits From

- VZKeyboardConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Keyboards

class VZKeyboardConfiguration

The base class for a configuring a keyboard.

class VZUSBKeyboardConfiguration

A device that defines the configuration for a USB keyboard.

