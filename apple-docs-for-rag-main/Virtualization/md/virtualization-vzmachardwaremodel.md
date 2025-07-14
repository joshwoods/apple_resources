

- Virtualization
-  VZMacHardwareModel 

Class

# VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

macOS 12.0+

``` source
class VZMacHardwareModel
```

## Mentioned in 

Installing macOS on a Virtual Machine

Using iCloud with macOS virtual machines

## Overview

The Mac hardware model abstracts a set of virtualized hardware elements and configurations.

A version of macOS may only run on certain hardware models. Additionally, the host may also only provide certain hardware models based on the version of macOS and the underlying hardware.

The isSupported property allows you to discover if the current host supports a particular hardware model.

Choosing the hardware model starts from a restore image with VZMacOSRestoreImage. A restore image describes its supported configuration requirements through its mostFeaturefulSupportedConfiguration property.

A configuration requirements object has a corresponding hardware model that you can use to configure a VM that meets the requirements. After obtaining the hardware model, use the platform configuration’s hardwareModel to configure the Mac platform object and use init(creatingStorageAt:hardwareModel:options:) to create its auxiliary storage.

After creating the VM, use VZMacOSInstaller to install macOS on it.

If you serialize the VM on disk, preserve the hardware model used for installation for subsequent boots. The dataRepresentation property provides a unique binary representation that you serialize to the file system. You can recreate the hardware model from the serialized binary representation with init(dataRepresentation:).

## Topics

### Creating the hardware model

init?(dataRepresentation: Data)

Creates an instance of the hardware model described by the specified data representation.

### Configuring the hardware model

var dataRepresentation: Data

Returns the opaque data representation of the hardware model.

var isSupported: Bool

A Boolean value that indicates whether the host supports this hardware model.

## Relationships

### Inherits From

- NSObject

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

class VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

class VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

### Platform components

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

class VZPlatformConfiguration

The base class for a platform configuration.

class VZMacMachineIdentifier

A unique identifier for a VM.

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

