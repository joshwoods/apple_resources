

- PCIDriverKit
- IOPCIDevice
-  MemoryRead16 

Instance Method

# MemoryRead16

Reads a 16-bit value synchronously from the PCI device’s aperture at the specified memory index.

DriverKitmacOS

``` source
void MemoryRead16(uint8_t memoryIndex, uint64_t offset, uint16_t * readData, IOOptionBits options);
```

## Parameters 

`memoryIndex`  

The index of the memory range from which to read.

`offset`  

An offset from the beginning of the specified memory range.

`readData`  

A variable in which to store the data. If this method encounters an error when reading the data, it sets the value to -1.

## See Also

### Reading and Writing Memory Locations

MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

MemoryRead8

Reads a 8-bit value synchronously from the PCI device’s aperture at the specified memory index.

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

