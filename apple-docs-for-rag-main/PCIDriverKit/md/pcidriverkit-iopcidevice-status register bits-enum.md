

- PCIDriverKit
- IOPCIDevice
-  Status Register Bits 

API Collection

# Status Register Bits

Constants that you use to access specific bits of the status register.

## Topics

### Registers

kIOPCIStatusInterrupt

The bit that contains the interrupt status.

kIOPCIStatusCapabilities

The bit that indicates the presence of an extended capability list item.

kIOPCIStatusPCI66

The bit that indicates the device is capable of 66 MHz operation.

kIOPCIStatusUDF

The bit that indicates the status of UDF support.

kIOPCIStatusFastBack2Back

The bit that indicates whether the device is capable of fast back-to-back transactions.

kIOPCIStatusTargetAbortCapable

The bit that indicates whether a function completed a posted or non-posted request as a completer abort error.

kIOPCIStatusTargetAbortActive

The bit that indicates whether a requester received a completion with a completer abort completion status.

kIOPCIStatusMasterAbortActive

The bit that indicates whether a requester received a completion with an unsupported request completion status

kIOPCIStatusSERRActive

The bit that indicates whether a function sent a fatal or nonfatal error message and set the SERR enable bit in the command register.

kIOPCIStatusParityErrActive

The bit that indicates whether a function received a poisoned transaction-layer packet.

kIOPCIStatusDevSel0

The DEVSEL timing status is set to 0.

kIOPCIStatusDevSel1

The DEVSEL timing status is set to 1.

kIOPCIStatusDevSel2

The DEVSEL timing status is set to 2.

kIOPCIStatusDevSel3

The DEVSEL timing status is set to 3.

### Constants

kIOPCIStatusLeadAbortActive

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

Bridge Header Offsets

Constants that specify offsets to distinct registers in a memory range.

Command Register Bits

Constants that you use to access specific bits of the command register.

