

- Endpoint Security
- es_event_mmap_t
-  flags 

Instance Property

# flags

Flags that affect the behavior of the memory mapping operation.

Mac CatalystmacOS

``` source
var flags: Int32
```

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The file to map memory into.

var file_pos: UInt64

The offset into the memory-map file.

var max_protection: Int32

The maximum value you can use for protection flags.

var protection: Int32

Options that affect the protection of mapped memory pages.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

