

- PCIDriverKit
-  IOPCIDevice 

Class

# IOPCIDevice

A DriverKit provider object that manages access to your custom PCI hardware.

DriverKitmacOS

``` source
class IOPCIDevice;
```

## Overview

Use an `IOPCIDevice` object to enable or manage the custom features of your PCI hardware. You don’t create instances of this class directly. Instead, the system creates an `IOPCIDevice` object and passes it to the IOService subclass of your custom driver. Use the methods of this object to read and write your hardware’s configuration settings. You can also use it to read and write any custom data in your device’s memory-mapped I/O.

Note

The endpoint driver is responsible for enabling the Memory Space Enable and Bus Master Enable settings each time it configures the PCI device. When a crash occurs, or when the system unloads your driver, the system disables these features.

## Topics

### Running the Service

init

Initializes the device.

Open

Opens a session to the PCI device.

Close

Closes the session to the PCI device.

free

Performs any final cleanup for the object.

### Reading and Writing Configuration Data

ConfigurationRead8

Reads an 8-bit data value synchronously from the device’s configuration space.

ConfigurationRead16

Reads a 16-bit data value synchronously from the device’s configuration space.

ConfigurationRead32

Reads a 32-bit data value synchronously from the device’s configuration space.

ConfigurationWrite8

Writes an 8-bit data value to the device’s configuration space.

ConfigurationWrite16

Writes an 16-bit data value to the device’s configuration space.

ConfigurationWrite32

Writes an 32-bit data value to the device’s configuration space.

Configuration Data Offsets

Constants for the offsets that you use to read and write configuration registers.

Bridge Header Offsets

Constants that specify offsets to distinct registers in a memory range.

Command Register Bits

Constants that you use to access specific bits of the command register.

Status Register Bits

Constants that you use to access specific bits of the status register.

### Reading and Writing Memory Locations

MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead16

Reads a 16-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead16

Reads a 16-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead32

Reads a 32-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead32

Reads a 32-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead64

Reads a 64-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead64

Reads a 64-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryWrite8

Writes an 8-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite8

Writes an 8-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite16

Writes an 16-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite16

Writes an 16-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite32

Writes an 32-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite32

Writes an 32-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

### Getting Device Information

FindPCICapability

Search the configuration space for a PCI capability register.

GetBusDeviceFunction

Returns the device’s bus, device, and function numbers.

PCI Capabilities

Constants that you use to get the capabilities of the PCI device.

Slot Capabilities

Constants that you use to get the slot-related capabilities of the PCI device.

### Managing Interrupts

Interrupt Types

Interrupt types that the device supports.

### Managing Power

HasPCIPowerManagement

Determines whether the device has the specified PCI bus power management capabilities.

EnablePCIPowerManagement

Configures the device’s PCI bus power management capabilities.

Power Management Capabilities

Constants you use to get and set the state of the device’s power management features.

Power Management Control/Status Register

Constants you use when checking bits in the power management register.

### Getting Error Codes

Correctable Error Bits

Constants for the bits in the correctable error status register.

Uncorrectable Error Bits

Constants for the bits in the uncorrectable error status register.

### Instance Methods

ClientCrashed

ConfigureInterrupts

GetBARInfo

GetLinkSpeed

Reset

RestoreDeviceState

SaveDeviceState

SetASPMState

SetLinkSpeed

SetProperties

## Relationships

### Inherits From

- IOService

## See Also

### Device Interface

Creating Custom PCIe Drivers for Thunderbolt Devices

Create a DriverKit extension to support your Thunderbolt device’s custom features.

