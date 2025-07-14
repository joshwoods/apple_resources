

- Paravirtualized Graphics
- PGDevice
-  mmioWrite(atOffset:value:) 

Instance Method

# mmioWrite(atOffset:value:)

Writes data to the virtual graphics device’s memory-mapped I/O region.

Mac Catalyst 14.0+macOS 11.0+

``` source
func mmioWrite(
    atOffset offset: Int,
    value: UInt32
)
```

**Required**

## Parameters 

`offset`  

The offset into the MMIO bar to write to.

`value`  

The value to write to memory.

## Discussion

Call this method whenever the guest virtual machine writes to the graphics device’s memory-mapped I/O region.

## See Also

### Handling Memory-Mapped I/O

func mmioRead(atOffset: Int) -> UInt32

Reads data from the virtual graphics device’s memory-mapped I/O region.

**Required**

