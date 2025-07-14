

- Virtualization
-  VZEFIBootLoader 

Class

# VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

macOS 13.0+

``` source
class VZEFIBootLoader
```

## Topics

### Creating an EFI boot loader

init()

Creates a new EFI boot loader.

### Instance properties

var variableStore: VZEFIVariableStore?

The boot loader’s EFI variable store.

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

class VZMacOSBootLoader

An object that loads and configures a boot loader for running macOS on Apple silicon as a guest system of your VM.

### Boot loaders

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

class VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

class VZEFIVariableStore

An object that represents the Extensible Firmware Interface (EFI) variable store that contains NVRAM variables the EFI exposes.

