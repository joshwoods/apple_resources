

- Virtualization
-  VZBootLoader 

Class

# VZBootLoader

The base class that defines the management of the initial process of the guest system.

macOS 11.0+

``` source
class VZBootLoader
```

## Overview

The VZBootLoader abstract class defines the common behaviors for booting a guest operating system into a VM. Don’t create instances of this class directly. Instead, instantiate the subclass that corresponds to the type of operating system you plan to load. For example, to create a boot loader object for a Linux kernel, create a VZLinuxBootLoader object; to create a boot loader object for installation using an ISO image create a VZEFIBootLoader. For a macOS system create VZMacOSBootLoader.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZEFIBootLoader
- VZLinuxBootLoader
- VZMacOSBootLoader

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

class VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

class VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

### Boot loaders

class VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

class VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

class VZEFIVariableStore

An object that represents the Extensible Firmware Interface (EFI) variable store that contains NVRAM variables the EFI exposes.

