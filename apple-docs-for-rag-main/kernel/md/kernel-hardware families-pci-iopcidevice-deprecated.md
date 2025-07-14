

- Kernel
- Hardware Families
- PCI
-  IOPCIDevice Deprecated

Class

# IOPCIDevice

An IOService class representing a PCI device.

macOS 10.0–11.0Deprecated

``` source
class IOPCIDevice : IOService
```

## Overview

The discovery of a PCI device by the PCI bus family results in an instance of the IOPCIDevice being created and published. It provides services for looking up and mapping memory mapped hardware, and access to the PCI configuration and I/O spaces.

Matching Supported by IOPCIDevice

Two types of matching are available, OpenFirmware name matching and PCI register matching. Currently, only one of these two matching schemes can be used in the same property table.

OpenFirmware Name Matching

IOService performs matching based on the IONameMatch property (see IOService). IOPCIDevices created with OpenFirmware device tree entries will name match based on the standard OpenFirmware name matching properties.

PCI Register Matching

A PCI device driver can also match on the values of certain config space registers.

In each case, several matching values can be specified, and an optional mask for the value of the config space register may follow the value, preceded by an '&' character.

kIOPCIMatchKey, "IOPCIMatch"

The kIOPCIMatchKey property matches the vendor and device ID (0x00) register, or the subsystem register (0x2c).

kIOPCIPrimaryMatchKey, "IOPCIPrimaryMatch"

The kIOPCIPrimaryMatchKey property matches the vendor and device ID (0x00) register.

kIOPCISecondaryMatchKey, "IOPCISecondaryMatch"

The kIOPCISecondaryMatchKey property matches the subsystem register (0x2c).

kIOPCIClassMatchKey, "IOPCIClassMatch"

The kIOPCIClassMatchKey property matches the class code register (0x08). The default mask for this register is 0xffffff00.

Examples:

&ltkey&gtIOPCIMatch&lt/key&gt

&ltstring&gt0x00261011&lt/string&gt

Matches a device whose vendor ID is 0x1011, and device ID is 0x0026, including subsystem IDs.

&ltkey&gtIOPCIMatch&lt/key&gt

&ltstring&gt0x00789004&0x00ffffff 0x78009004&0x0xff00ffff&lt/string&gt

Matches with any device with a vendor ID of 0x9004, and a device ID of 0xzz78 or 0x78zz, where 'z' is don't care.

&ltkey&gtIOPCIClassMatch&lt/key&gt

&ltstring&gt0x02000000&0xffff0000&lt/string&gt

Matches a device whose class code is 0x0200zz, an ethernet device.

## Topics

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

### Instance Variables

reserved

### Instance Methods

- ClientCrashed_Impl

- Close

Closes the session to the PCI device.

- ConfigurationRead16

Reads a 16-bit data value synchronously from the device’s configuration space.

- ConfigurationRead32

Reads a 32-bit data value synchronously from the device’s configuration space.

- ConfigurationRead8

Reads an 8-bit data value synchronously from the device’s configuration space.

- ConfigurationWrite16

Writes an 16-bit data value to the device’s configuration space.

- ConfigurationWrite32

Writes an 32-bit data value to the device’s configuration space.

- ConfigurationWrite8

Writes an 8-bit data value to the device’s configuration space.

- ConfigureInterrupts

- ConfigureInterrupts_Impl

- Dispatch

- EnablePCIPowerManagement

- EnablePCIPowerManagement_Impl

- FindPCICapability

- FindPCICapability_Impl

- GetBARInfo

- GetBARInfo_Impl

- GetBusDeviceFunction

- GetBusDeviceFunction_Impl

- GetLinkSpeed

- GetLinkSpeed_Impl

- HasPCIPowerManagement

- HasPCIPowerManagement_Impl

- MemoryRead16

Reads a 16-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead16

Reads a 16-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead32

Reads a 32-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead32

Reads a 32-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead64

Reads a 64-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead64

Reads a 64-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

- MemoryWrite16

Writes an 16-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite16

Writes an 16-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite32

Writes an 32-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite32

Writes an 32-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite8

Writes an 8-bit value to the PCI device’s aperture at the specified memory index.

- MemoryWrite8

Writes an 8-bit value to the PCI device’s aperture at the specified memory index.

- Open

Opens a session to the PCI device.

- Reset

- Reset_Impl

- RestoreDeviceState

- RestoreDeviceState_Impl

- SaveDeviceState

- SaveDeviceState_Impl

- SetASPMState

- SetASPMState_Impl

- SetLinkSpeed

- SetLinkSpeed_Impl

- SetProperties_Impl

- addPowerChild

- attach

- callPlatformFunction

- callPlatformFunction

- checkLink

- compareName

- completeFLR

- configAccess

- configRead16

- configRead16

- configRead32

- configRead32

- configRead8

- configRead8

- configWrite16

- configWrite16

- configWrite16Filter

- configWrite32

- configWrite32

- configWrite32Filter

- configWrite8

- configWrite8

- configWrite8Filter

- configureInterrupts

- copyAERErrorDescriptionForBit

- createEventSource

- detach

- detachAbove

- detachFromChild

- deviceMemoryRead

- deviceMemoryRead16

- deviceMemoryRead16

- deviceMemoryRead32

- deviceMemoryRead32

- deviceMemoryRead64

- deviceMemoryRead64

- deviceMemoryRead8

- deviceMemoryRead8

- deviceMemoryWrite

- deviceMemoryWrite16

- deviceMemoryWrite16

- deviceMemoryWrite32

- deviceMemoryWrite32

- deviceMemoryWrite64

- deviceMemoryWrite64

- deviceMemoryWrite8

- deviceMemoryWrite8

- enableACS

- enableLTR

- enablePCIPowerManagement

- extendedConfigRead16

- extendedConfigRead32

- extendedConfigRead8

- extendedConfigWrite16

- extendedConfigWrite32

- extendedConfigWrite8

- extendedFindPCICapability

- findPCICapability

- flr

- free

Performs any final cleanup for the object.

- getBusNumber

- getDeviceMemoryWithIndex

- getDeviceMemoryWithRegister

- getDeviceNumber

- getFunctionNumber

- getLinkSpeed

- getMetaClass

- getProperty

- getResources

- handleClose

- handleOpen

- hasPCIPowerManagement

- init

- init

- initReserved

- initialPowerStateForDomainState

- ioDeviceMemory

- ioRead16

- ioRead32

- ioRead8

- ioWrite16

- ioWrite32

- ioWrite8

- isDownstreamFacing

- kernelRequestProbe

- launchReprobeThread

- mapDeviceMemoryWithRegister

- matchLocation

- matchPropertyTable

- matchPropertyTable

- maxCapabilityForDomainState

- newUserClient

- powerStateForDomainState

- powerStateWillChangeTo

- powerStateWillChangeToGated

- prepareFLR

- protectDevice

- registerCrashNotification

- relocate

- removePowerChild

- reprobeThreadCall

- requestProbe

- reset

- resetFunction

- resetNubState

- restoreDeviceState

- saveDeviceState

- setASPMState

- setBusLeadEnable

- setBusMasterEnable

- setConfigBits

- setConfigHandler

- setIOEnable

- setLatencyTolerance

- setLinkSpeed

- setMemoryEnable

- setPCIPowerState

- setPowerState

- setPowerStateGated

- setProperties

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- setTunnelL1Enable

- shouldSkipReset

- supportsFLR

- unregisterCrashNotification

- updateWakeReason

### Type Methods

+ ConfigureInterrupts_Invoke

+ EnablePCIPowerManagement_Invoke

+ FindPCICapability_Invoke

+ GetBARInfo_Invoke

+ GetBusDeviceFunction_Invoke

+ GetLinkSpeed_Invoke

+ HasPCIPowerManagement_Invoke

+ Reset_Invoke

+ RestoreDeviceState_Invoke

+ SaveDeviceState_Invoke

+ SetASPMState_Invoke

+ SetLinkSpeed_Invoke

+ getCloseCommandMask

+ hasL1Errata

## Relationships

### Inherits From

- IOService

## See Also

### Devices

Implementing a PCIe Kext for a Thunderbolt Device

Create an IOKit driver to support Thunderbolt devices that implement features not supported in PCIDriverKit, such as wireless networking or audio.

IOAGPDevice

An IOService class representing an AGP primary device.

Deprecated

