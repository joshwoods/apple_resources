

- Virtualization
-  VZGenericMachineIdentifier 

Class

# VZGenericMachineIdentifier

An object that represents a unique identifier for a virtual machine.

macOS 13.0+

``` source
class VZGenericMachineIdentifier
```

## Overview

Use the data representation in dataRepresentation to save the VM’s identifier. To restore a previously saved identifier use init(dataRepresentation:).

## Topics

### Creating a Machine Identifier

init()

Creates a new unique identifier for a VM.

init?(dataRepresentation: Data)

Creates a new unique identifier for a VM with the provided data.

### Getting Information About the Machine Identifier

var dataRepresentation: Data

An opaque data representation of the VM’s identifier.

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

### Identifying the platform configuration

var machineIdentifier: VZGenericMachineIdentifier

A value that represents a unique identifier for the virtual machine.

var isNestedVirtualizationEnabled: Bool

A Boolean value that indicates whether nested virtualization is in an enabled state.

class var isNestedVirtualizationSupported: Bool

A Boolean value that describes whether the platform configuration supports nested virtualization.

