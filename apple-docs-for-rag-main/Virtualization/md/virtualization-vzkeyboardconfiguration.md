

- Virtualization
-  VZKeyboardConfiguration 

Class

# VZKeyboardConfiguration

The base class for a configuring a keyboard.

macOS 12.0+

``` source
class VZKeyboardConfiguration
```

## Overview

`VZKeyboardConfiguration` defines the abstract interface that defines a virtual keyboard that you connect to a guest operating system. Don’t instantiate `VZKeyboardConfiguration` directly, use one of its subclasses such as VZUSBKeyboardConfiguration instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacKeyboardConfiguration
- VZUSBKeyboardConfiguration

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

class VZMacKeyboardConfiguration

A device that defines the configuration for a Mac keyboard.

class VZUSBKeyboardConfiguration

A device that defines the configuration for a USB keyboard.

