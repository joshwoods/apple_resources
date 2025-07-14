

- Kernel
- Hardware Families
- PCI
-  IOAGPDevice Deprecated

Class

# IOAGPDevice

An IOService class representing an AGP primary device.

macOS 10.0–11.0Deprecated

``` source
class IOAGPDevice : IOPCIDevice
```

## Overview

The discovery of an AGP primary device by the PCI bus family results in an instance of the IOAGPDevice being created and published. It provides services specific to AGP, in addition to the PCI services supplied by its superclass IOPCIDevice.

## Topics

### Miscellaneous

commitAGPMemory

Makes memory addressable by AGP transactions.

createAGPSpace

Allocates the AGP space, and enables AGP transactions on the primary and secondary.

destroyAGPSpace

Destroys the AGP space, and disables AGP transactions on the primary and secondary.

getAGPRangeAllocator

Accessor to obtain the AGP range allocator.

getAGPSpace

Returns the allocated AGP space.

getAGPStatus

Returns the current state of the AGP bus.

releaseAGPMemory

Releases memory addressable by AGP transactions.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- commitAGPMemory

- createAGPSpace

- destroyAGPSpace

- getAGPRangeAllocator

- getAGPSpace

- getAGPStatus

- getMetaClass

- releaseAGPMemory

- resetAGP

## Relationships

### Inherits From

- IOPCIDevice

## See Also

### Devices

Implementing a PCIe Kext for a Thunderbolt Device

Create an IOKit driver to support Thunderbolt devices that implement features not supported in PCIDriverKit, such as wireless networking or audio.

IOPCIDevice

An IOService class representing a PCI device.

Deprecated

