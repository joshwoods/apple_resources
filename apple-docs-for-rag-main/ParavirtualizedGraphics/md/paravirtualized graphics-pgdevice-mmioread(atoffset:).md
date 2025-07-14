

- Paravirtualized Graphics
- PGDevice
-  mmioRead(atOffset:) 

Instance Method

# mmioRead(atOffset:)

Reads data from the virtual graphics device’s memory-mapped I/O region.

Mac Catalyst 14.0+macOS 11.0+

``` source
func mmioRead(atOffset offset: Int) -> UInt32
```

**Required**

## Parameters 

`offset`  

The offset into the MMIO bar to write to.

## Return Value

The 32-bit unsigned integer from the MMIO region.

## Discussion

Call this method whenever the guest virtual machine reads from the graphics device’s memory-mapped I/O region.

## See Also

### Handling Memory-Mapped I/O

func mmioWrite(atOffset: Int, value: UInt32)

Writes data to the virtual graphics device’s memory-mapped I/O region.

**Required**

