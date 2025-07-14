

- PCIDriverKit
- IOPCIDevice
-  ConfigurationRead32 

Instance Method

# ConfigurationRead32

Reads a 32-bit data value synchronously from the device’s configuration space.

DriverKitmacOS

``` source
void ConfigurationRead32(uint64_t offset, uint32_t * readData);
```

## Parameters 

`offset`  

An offset into the configuration space. This method ignores bits 0 and 1. For a list of possible offset values, see Configuration Data Offsets.

`readData`  

A variable that stores the 32-bit data value. If the method encounters an error, it sets the value to -1.

## See Also

### Reading and Writing Configuration Data

ConfigurationRead8

Reads an 8-bit data value synchronously from the device’s configuration space.

ConfigurationRead16

Reads a 16-bit data value synchronously from the device’s configuration space.

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

