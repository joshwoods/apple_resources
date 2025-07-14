

- PCIDriverKit
- IOPCIDevice
-  Bridge Header Offsets 

API Collection

# Bridge Header Offsets

Constants that specify offsets to distinct registers in a memory range.

## Topics

### Offsets

kPCI2PCIOffsetPrimaryBus

The offset to the primary bus number register.

kPCI2PCIOffsetSecondaryBus

The offset to the secondary bus number register.

kPCI2PCIOffsetSubordinateBus

The offset to the subordinate bus number register.

kPCI2PCIOffsetSecondaryLT

The offset to the secondary latency timer register.

kPCI2PCIOffsetIORange

The offset to the I/O base upper and I/O limit upper registers.

kPCI2PCIOffsetMemoryRange

The offset to the memory base and memory limit registers.

kPCI2PCIOffsetPrefetchMemoryRange

The offset to the prefetchable memory base and prefetchable memory limit registers.

kPCI2PCIOffsetPrefetchUpperBase

The offset to the prefetchable base upper 32 bits register.

kPCI2PCIOffsetPrefetchUpperLimit

The offset to the prefetchable limit upper 32 bits registers.

kPCI2PCIOffsetUpperIORange

The offset to the I/O base upper and I/O limit upper registers.

kPCI2PCIOffsetBridgeControl

The offset to the bridge control register.

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

Configuration Data Offsets

Constants for the offsets that you use to read and write configuration registers.

Command Register Bits

Constants that you use to access specific bits of the command register.

Status Register Bits

Constants that you use to access specific bits of the status register.

