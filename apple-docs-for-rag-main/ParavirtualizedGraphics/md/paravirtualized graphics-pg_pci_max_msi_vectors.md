

- Paravirtualized Graphics
-  PG_PCI_MAX_MSI_VECTORS 

Global Variable

# PG_PCI_MAX_MSI_VECTORS

The number of MSI vectors that you need to allocate for the graphics configuration.

Mac Catalyst 14.0+macOS 11.0+

``` source
var PG_PCI_MAX_MSI_VECTORS: Int32 { get }
```

## See Also

### PCI Device Characteristics

var PG_PCI_DEVICE_ID: Int32

The PCI device identifier to use when advertising the graphics stack inside a virtual machine.

var PG_PCI_VENDOR_ID: Int32

The vendor identifier to use when advertising the graphics stack inside a virtual machine.

var PG_PCI_BAR_MMIO: Int32

The base address register to use when advertising the graphics stack inside a virtual machine.

func PGCopyOptionROMURL() -> URL

Copies the URL of the ROM image to use on the guest graphics device.

