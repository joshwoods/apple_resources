

- Endpoint Security
- es_event_mmap_t
-  max_protection 

Instance Property

# max_protection

The maximum value you can use for protection flags.

Mac CatalystmacOS

``` source
var max_protection: Int32
```

## Discussion

This value uses the protection flags defined by `mmap(2)`, such as `PROT_READ` and `PROT_WRITE`. You can use the definitions for these flags found in `sys/mman.h` in the macOS SDK inside of the Xcode app bundle.

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The file to map memory into.

var file_pos: UInt64

The offset into the memory-map file.

var flags: Int32

Flags that affect the behavior of the memory mapping operation.

var protection: Int32

Options that affect the protection of mapped memory pages.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

