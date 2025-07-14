

- Virtualization
-  VZMacAuxiliaryStorage 

Class

# VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

macOS 12.0+

``` source
class VZMacAuxiliaryStorage
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Overview

The Mac auxiliary storage contains data used by the boot loader and the guest operating system. It’s necessary to boot a macOS guest OS.

When creating a new VM, use init(creatingStorageAt:hardwareModel:options:) to create a default initialized auxiliary storage.

The hardware model you use when creating the new auxiliary storage depends on the restore image that you’ll use for installation. From the restore image, use mostFeaturefulSupportedConfiguration to get a supported configuration. A configuration has a VZMacHardwareModel associated with it.

After initializing the new auxiliary storage, set it on `VZMacPlatformConfiguration`.auxiliaryStorage.

The hardware model in `VZMacPlatformConfiguration`.hardwareModel must be identical to the one used to create the empty auxiliary storage., otherwise the behavior isn’t defined.

When installing macOS, the VZMacOSInstaller lays out data on the auxiliary storage. After installation, the macOS guest uses the auxiliary storage for every subsequent boot.

When moving or performing a backup of a VM, you must move or copy the file containing the auxiliary storage along with the main disk image.

To boot a VM created with `VZMacOSInstaller`, use init(contentsOfURL:) to set up the auxiliary storage from the existing file used during installation.

When using an existing file, the hardware model of the `VZMacPlatformConfiguration`.hardwareModel must match the hardware model used when creating the original file.

## Topics

### Creating the auxiliary storage

init(contentsOfURL: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

Deprecated

init(url: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

init(creatingStorageAt: URL, hardwareModel: VZMacHardwareModel, options: VZMacAuxiliaryStorage.InitializationOptions) throws

Creates an initialized Mac auxiliary storage instance that describes a specific hardware model at a URL you specify.

struct InitializationOptions

Options you can set when creating new auxiliary storage.

### Configuring the auxiliary storage location

var url: URL

The URL of the auxiliary storage on the local file system.

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

class VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

class VZMacOSConfigurationRequirements

An object that describes the parameter constraints required by a specific configuration of macOS.

class VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

### Platform components

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

class VZPlatformConfiguration

The base class for a platform configuration.

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

class VZMacMachineIdentifier

A unique identifier for a VM.

