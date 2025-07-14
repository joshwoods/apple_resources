

- Paravirtualized Graphics
-  PG_PCI_BAR_MMIO 

Global Variable

# PG_PCI_BAR_MMIO

The base address register to use when advertising the graphics stack inside a virtual machine.

Mac Catalyst 14.0+macOS 11.0+

``` source
var PG_PCI_BAR_MMIO: Int32 { get }
```

## Discussion

Specify the following characteristics for the memory that this base address register references:

- Allocate 16 kilobytes of memory.

- Place MSI interrupt vectors between offsets `0x0000` and `0x0FFF` of this memory block.

- Place MMIO mapped registers starting at offset `0x1000`.

When you see a read or write access to this memory region, call mmioRead(atOffset:) or mmioWrite(atOffset:value:) on the host device. The framework aligns reads and writes to addresses that are multiples of `4` bytes with a length of `4` bytes.

## See Also

### PCI Device Characteristics

var PG_PCI_DEVICE_ID: Int32

The PCI device identifier to use when advertising the graphics stack inside a virtual machine.

var PG_PCI_VENDOR_ID: Int32

The vendor identifier to use when advertising the graphics stack inside a virtual machine.

var PG_PCI_MAX_MSI_VECTORS: Int32

The number of MSI vectors that you need to allocate for the graphics configuration.

func PGCopyOptionROMURL() -> URL

Copies the URL of the ROM image to use on the guest graphics device.

