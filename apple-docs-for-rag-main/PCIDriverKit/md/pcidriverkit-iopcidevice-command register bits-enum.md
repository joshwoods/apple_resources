

- PCIDriverKit
- IOPCIDevice
-  Command Register Bits 

API Collection

# Command Register Bits

Constants that you use to access specific bits of the command register.

## Topics

### Bits

kIOPCICommandIOSpace

The bit that indicates whether the device allows access to I/O space.

kIOPCICommandMemorySpace

The bit that indicates whether the device allows access to memory space.

kIOPCICommandBusMaster

The bit that controls the ability to issue or forward memory and I/O requests.

kIOPCICommandSpecialCycles

The bit that enables the legacy special cycle feature.

kIOPCICommandMemWrInvalidate

The bit that enables legacy memory writing and invalidation.

kIOPCICommandPaletteSnoop

The bit that enables the legacy palette snooping feature.

kIOPCICommandParityError

The bit that controls the logging of poisoned transaction-layer packets.

kIOPCICommandAddressStepping

The bit that controls the legacy address stepping and wait cycle feature.

kIOPCICommandSERR

The bit that enables the upstream reporting of fatal and non-fatal errors.

kIOPCICommandFastBack2Back

The bit that enables legacy fast back-to-back transactions.

kIOPCICommandInterruptDisable

The bit that prevents the generation of INTx emulation interrupts.

kIOPCICommandBusLead

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

Status Register Bits

Constants that you use to access specific bits of the status register.

