

- PCIDriverKit
- IOPCIDevice
-  Configuration Data Offsets 

API Collection

# Configuration Data Offsets

Constants for the offsets that you use to read and write configuration registers.

## Topics

### Offsets

kIOPCIConfigurationOffsetVendorID

The offset to the 16-bit value that identifies the manufacturer of the device.

kIOPCIConfigurationOffsetDeviceID

The offset to the 16-bit value that the manufacturer uses to identify the particular function.

kIOPCIConfigurationOffsetCommand

The offset to the 16-bit value that defines how the device responds to commands.

kIOPCIConfigurationOffsetStatus

The offset to the 16-bit value that contains the status of the device.

kIOPCIConfigurationOffsetRevisionID

The offset to the 8-bit value that the manufacturer uses to identify the revision of the device.

kIOPCIConfigurationOffsetClassCode

The offset to the 24-bit, read-only value that identifies the generic operation of the device.

kIOPCIConfigurationOffsetCacheLineSize

The offset to the 8-bit value that contains legacy information about the cache line size.

kIOPCIConfigurationOffsetLatencyTimer

The offset to the 8-bit value that containsn legacy information for devices with a primary latency timer.

kIOPCIConfigurationOffsetHeaderType

The offset to the 8-bit value that defines the layout of the second part of the predefined header.

kIOPCIConfigurationOffsetBIST

The offset to the 8-bit value that controls and reports the status of the device’s built-in, self-test behavior.

kIOPCIConfigurationOffsetBaseAddress0

The offset to the 32-bit value for base address 0.

kIOPCIConfigurationOffsetBaseAddress1

The offset to the 32-bit value for base address 1.

kIOPCIConfigurationOffsetBaseAddress2

The offset to the 32-bit value for base address 2.

kIOPCIConfigurationOffsetBaseAddress3

The offset to the 32-bit value for base address 3.

kIOPCIConfigurationOffsetBaseAddress4

The offset to the 32-bit value for base address 4.

kIOPCIConfigurationOffsetBaseAddress5

The offset to the 32-bit value for base address 5.

kIOPCIConfigurationOffsetCardBusCISPtr

The offset to the 32-bit read-only value that describes legacy PCI functionality.

kIOPCIConfigurationOffsetSubSystemVendorID

The offset to the 16-bit value that identifies the manufacturer of a device containing common PCI components.

kIOPCIConfigurationOffsetSubSystemID

The offset to the 16-bit value that identifies a specific device that uses common PCI components.

kIOPCIConfigurationOffsetExpansionROMBase

The offset to the 32-bit value that contains the base address and size of the device’s expansion ROM.

kIOPCIConfigurationOffsetCapabilitiesPtr

The offset to the 8-bit value that points to the linked list of capabilities the device implements.

kIOPCIConfigurationOffsetInterruptLine

The offset to the 8-bit value that contains interrupt line-routing information.

kIOPCIConfigurationOffsetInterruptPin

The offset to the 8-bit read-only value that identifies the device’s supported interrupt messages.

kIOPCIConfigurationOffsetMinimumGrant

The offset to the 8-bit value that contains legacy PCI information about the minimum grant.

kIOPCIConfigurationOffsetMaximumLatency

The offset to the 8-bit value that contains legacy PCI information about the maximum latency.

## See Also

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

Bridge Header Offsets

Constants that specify offsets to distinct registers in a memory range.

Command Register Bits

Constants that you use to access specific bits of the command register.

Status Register Bits

Constants that you use to access specific bits of the status register.

