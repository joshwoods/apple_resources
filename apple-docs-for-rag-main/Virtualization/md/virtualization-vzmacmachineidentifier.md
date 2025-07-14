

- Virtualization
-  VZMacMachineIdentifier 

Class

# VZMacMachineIdentifier

A unique identifier for a VM.

macOS 12.0+

``` source
class VZMacMachineIdentifier
```

## Overview

This value uniquely identifies a virtual Mac hardware instance. Two VMs running concurrently shouldn’t use the same identifier.

When serializing the VM to disk, you can preserve the identifier in a binary representation by serializing the data in the `VZMacMachineIdentifier`.dataRepresentation property. Conversely, you can recreate the identifier with init(dataRepresentation:) from the binary representation.

You can compare the contents of two identifiers with isEqual(to:).

## Topics

### Creating a machine identifier

init?(dataRepresentation: Data)

Create a machine identifier described by the specified data representation.

init()

Creates a new unique machine identifier.

### Machine data representation

var dataRepresentation: Data

Returns the opaque data representation of the machine identifier.

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

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

