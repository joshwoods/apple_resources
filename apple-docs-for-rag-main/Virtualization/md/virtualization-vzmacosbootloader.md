

- Virtualization
-  VZMacOSBootLoader 

Class

# VZMacOSBootLoader

An object that loads and configures a boot loader for running macOS on Apple silicon as a guest system of your VM.

macOS 12.0+

``` source
class VZMacOSBootLoader
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Overview

You must use a VZMacPlatformConfiguration in conjunction with the macOS boot loader. It’s invalid to use it with any other platform configuration.

## Topics

### Creating a macOS boot loader

init()

Creates a macOS boot loader.

## Relationships

### Inherits From

- VZBootLoader

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

var platform: VZPlatformConfiguration

The hardware platform to use.

### Boot images

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

