

- PCIDriverKit
- IOPCIDevice
-  MemoryWrite32 

Instance Method

# MemoryWrite32

Writes an 32-bit value to the PCI device’s aperture at the specified memory index.

DriverKitmacOS

``` source
void MemoryWrite32(uint8_t memoryIndex, uint64_t offset, uint32_t data, IOOptionBits options);
```

## Parameters 

`memoryIndex`  

The index of the memory range from which to read.

`offset`  

An offset from the beginning of the specified memory range.

`data`  

The data that you want to write to the specified location.

## See Also

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

MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

MemoryWrite64

Writes an 64-bit value to the PCI device’s aperture at the specified memory index.

