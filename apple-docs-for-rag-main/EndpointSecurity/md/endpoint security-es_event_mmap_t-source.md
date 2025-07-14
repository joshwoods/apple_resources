

- Endpoint Security
- es_event_mmap_t
-  source 

Instance Property

# source

The file to map memory into.

Mac CatalystmacOS

``` source
var source: UnsafeMutablePointer
```

## See Also

### Inspecting Event Properties

var file_pos: UInt64

The offset into the memory-map file.

var flags: Int32

Flags that affect the behavior of the memory mapping operation.

var max_protection: Int32

The maximum value you can use for protection flags.

var protection: Int32

Options that affect the protection of mapped memory pages.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

