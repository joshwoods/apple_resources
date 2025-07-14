

- Virtualization
-  VZEFIVariableStore 

Class

# VZEFIVariableStore

An object that represents the Extensible Firmware Interface (EFI) variable store that contains NVRAM variables the EFI exposes.

macOS 13.0+

``` source
class VZEFIVariableStore
```

## Topics

### Creating the variable store

init(creatingVariableStoreAt: URL, options: VZEFIVariableStore.InitializationOptions) throws

Creates a new EFI variable store at specified the URL on the filesystem, initialization options, and error-return variable.

init(url: URL)

Initialize the variable store from the URL of an existing file.

struct InitializationOptions

Constants that describe the options available when creating a new Extensible Firmware Interface (EFI) variable store.

### Instance properties

var url: URL

The URL of the variable store on the local file system.

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

### Boot loaders

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

class VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

class VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

