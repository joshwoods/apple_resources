

- Kernel
- Hardware Families
- PCI
- IOPCIDevice
-  configWrite16 

# configWrite16

Writes a 16-bit value to the PCI device's configuration space.

``` source
void configWrite16(
 IOByteCountoffset,
 UInt16data ) 
```

## Parameters 

`offset`  

An offset into configuration space, of which bit 0 is ignored.

`data`  

An 16-bit value to be written in host byte order (big endian on PPC).

## Overview

This method write a 16-bit value to a configuration space register on the device.

## See Also

### Miscellaneous

configRead16

Reads a 16-bit value from the PCI device's configuration space.

configRead32

Reads a 32-bit value from the PCI device's configuration space.

configRead8

Reads a 8-bit value from the PCI device's configuration space.

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

findPCICapability

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

