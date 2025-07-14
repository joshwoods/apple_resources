

- PCIDriverKit
- IOPCIDevice
-  ConfigurationWrite16 

Instance Method

# ConfigurationWrite16

Writes an 16-bit data value to the device’s configuration space.

DriverKitmacOS

``` source
void ConfigurationWrite16(uint64_t offset, uint16_t data);
```

## Parameters 

`offset`  

An offset into the configuration space. This method ignores bits 0 and 1. For a list of possible offset values, see Configuration Data Offsets.

`data`  

The data value that you want DriverKit to write to the specified location.

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

