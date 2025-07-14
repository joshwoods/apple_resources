

- Virtualization
-  VZUSBKeyboardConfiguration 

Class

# VZUSBKeyboardConfiguration

A device that defines the configuration for a USB keyboard.

macOS 12.0+

``` source
class VZUSBKeyboardConfiguration
```

## Overview

A VZVirtualMachineView can use this device to send key events to the VM.

## Topics

### Creating a USB keyboard

init()

Creates a USB keyboard configuration.

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

class VZMacKeyboardConfiguration

A device that defines the configuration for a Mac keyboard.

