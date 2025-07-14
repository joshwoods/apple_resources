

- Kernel
- Hardware Families
- PCI
- IOPCIDevice
-  enablePCIPowerManagement 

# enablePCIPowerManagement

enable PCI power management for sleep state

``` source
virtual IOReturn enablePCIPowerManagement(
 IOOptionBits state = 0xffffffff); 
```

## Parameters 

`state(optional)`  

Enables PCI Power Management by placing the function in the given state (e.g. kPCIPMCSPowerStateD3). If state is not specified or is 0xffffffff, then the IOPCIDevice determines the desired state. If state is kPCIPMCSPowerStateD0 (0) then PCI Power Management is disabled.

## Return Value

kIOReturnSuccess if there were no errors

## Overview

This method will enable PCI Bus Powermanagement when going to sleep mode.

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

