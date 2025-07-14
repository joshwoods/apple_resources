

- Kernel
- Hardware Families
- PCI
- IOPCIDevice
-  hasPCIPowerManagement 

# hasPCIPowerManagement

determine whether or not the device supports PCI Bus Power Management.

``` source
virtual bool hasPCIPowerManagement(
 IOOptionBits state = 0); 
```

## Parameters 

`state(optional)`  

Check for support of a specific state (e.g. kPCIPMCPMESupportFromD3Cold). If state is not suuplied or is 0, then check for a property in the registry which tells which state the hardware expects the device to go to during sleep.

## Return Value

true if the specified state is supported

## Overview

This method will look at the device's capabilties registers and determine whether or not the device supports the PCI BUS Power Management Specification.

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

