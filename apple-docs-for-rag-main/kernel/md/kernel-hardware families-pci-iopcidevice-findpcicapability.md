

- Kernel
- Hardware Families
- PCI
- IOPCIDevice
-  findPCICapability 

# findPCICapability

Search configuration space for a PCI capability register.

``` source
virtual UInt32 findPCICapability(
 UInt8 capabilityID,
 UInt8 *offset = 0 ); 
```

## Parameters 

`capabilityID`  

An 8-bit PCI capability ID.

`offset`  

An optional pointer to return the offset into config space where the capability was found.

## Return Value

The 32-bit value of the capability register if one was found, zero otherwise.

## Overview

This method searches the device's config space for a PCI capability register matching the passed capability ID, if the device supports PCI capabilities. To search for PCI Express extended capabilities or for multiple capablities with the same ID, use the extendedFindPCICapability() method.

## See Also

### Miscellaneous

configRead16

Reads a 16-bit value from the PCI device's configuration space.

configRead32

Reads a 32-bit value from the PCI device's configuration space.

configRead8

Reads a 8-bit value from the PCI device's configuration space.

configWrite16

Writes a 16-bit value to the PCI device's configuration space.

configWrite32

Writes a 32-bit value to the PCI device's configuration space.

configWrite8

Writes a 8-bit value to the PCI device's configuration space.

enablePCIPowerManagement

enable PCI power management for sleep state

extendedConfigRead16

Reads a 16-bit value from the PCI device's configuration space.

extendedConfigRead32

Reads a 32-bit value from the PCI device's configuration space.

extendedConfigRead8

Reads a 8-bit value from the PCI device's configuration space.

extendedConfigWrite16

Writes a 16-bit value to the PCI device's configuration space.

extendedConfigWrite32

Writes a 32-bit value to the PCI device's configuration space.

extendedConfigWrite8

Writes a 8-bit value to the PCI device's configuration space.

extendedFindPCICapability

Search configuration space for a PCI capability register.

getBusNumber

Accessor to return the PCI device's assigned bus number.

getDeviceMemoryWithRegister

Returns an instance of IODeviceMemory representing one of the device's memory mapped ranges.

getDeviceNumber

Accessor to return the PCI device's device number.

getFunctionNumber

Accessor to return the PCI device's function number.

hasPCIPowerManagement

determine whether or not the device supports PCI Bus Power Management.

ioDeviceMemory

Accessor to the I/O space aperture for the bus.

ioRead16

Reads a 16-bit value from an I/O space aperture.

ioRead32

Reads a 32-bit value from an I/O space aperture.

ioRead8

Reads a 8-bit value from an I/O space aperture.

ioWrite16

Writes a 16-bit value to an I/O space aperture.

ioWrite32

Writes a 32-bit value to an I/O space aperture.

ioWrite8

Writes a 8-bit value to an I/O space aperture.

mapDeviceMemoryWithRegister

Maps a physical range of the device.

setBusMasterEnable

Enables bus mastering on the device.

setConfigBits

Sets masked bits in a configuration space register.

setIOEnable

Sets the device's I/O space response.

setMemoryEnable

Sets the device's memory space response.

