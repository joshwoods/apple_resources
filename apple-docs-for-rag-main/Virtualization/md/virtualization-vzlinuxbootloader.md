

- Virtualization
-  VZLinuxBootLoader 

Class

# VZLinuxBootLoader

An object that loads and configures a Linux kernel as the guest system of your VM.

macOS 11.0+

``` source
class VZLinuxBootLoader
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

## Overview

Create and configure a VZLinuxBootLoader object during the initial configuration of your VM. Use this object to specify the location of the Linux kernel that serves as the guest operating system. You can also specify additional information to use during the boot process, such as command-line parameters to pass to the kernel. Assign the VZLinuxBootLoader object to the bootLoader property of your VZVirtualMachineConfiguration object.  A configuration with `VZLinuxBootLoader` is only valid if used with VZGenericPlatformConfiguration.

## Topics

### Creating the Linux boot loader

init(kernelURL: URL)

Creates a boot loader that launches the Linux kernel at the specified URL.

### Configuring the boot parameters

var commandLine: String

The command-line parameters to pass to the Linux kernel at boot time.

var initialRamdiskURL: URL?

The location of an optional RAM disk, which the boot loader maps into memory before it boots the Linux kernel.

### Getting the kernel file

var kernelURL: URL

The URL of the Linux kernel file.

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

class VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

### Boot loaders

class VZBootLoader

The base class that defines the management of the initial process of the guest system.

class VZEFIBootLoader

The boot loader configuration the system uses to boot guest-operating systems that expect an Extensible Firmware Interface (EFI) ROM.

class VZEFIVariableStore

An object that represents the Extensible Firmware Interface (EFI) variable store that contains NVRAM variables the EFI exposes.

