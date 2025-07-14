

- Virtualization
-  VZMacPlatformConfiguration 

Class

# VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

macOS 12.0+

``` source
class VZMacPlatformConfiguration
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Overview

When creating a VM, the hardwareModel and auxiliaryStorage depend on the restore image that you use to install macOS.

To choose the hardware model, start from `VZMacOSRestoreImage`.mostFeaturefulSupportedConfiguration to get a supported configuration, then use its `VZMacOSConfigurationRequirements`.hardwareModel property to get the hardware model.

Use the hardware model to set up `VZMacPlatformConfiguration` and to initialize a new auxiliary storage with init(creatingStorageAt:hardwareModel:options:).

When you save a VM to disk and load it again, you must restore the hardwareModel, machineIdentifier and auxiliaryStorage properties to their original values.

If you create multiple VMs from the same configuration, each should have a unique `auxiliaryStorage` and `machineIdentifier`.

## Topics

### Creating a platform configuration

init()

Creates a new Mac platform configuration.

### Getting platform properties

var auxiliaryStorage: VZMacAuxiliaryStorage?

The Mac auxiliary storage.

var hardwareModel: VZMacHardwareModel

The Mac hardware model.

var machineIdentifier: VZMacMachineIdentifier

The Mac machine identifier.

## Relationships

### Inherits From

- VZPlatformConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Platform components

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

class VZPlatformConfiguration

The base class for a platform configuration.

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

class VZMacMachineIdentifier

A unique identifier for a VM.

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

