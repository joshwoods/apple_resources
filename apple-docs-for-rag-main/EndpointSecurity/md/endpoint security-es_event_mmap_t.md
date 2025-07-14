

- Endpoint Security
-  es_event_mmap_t 

Structure

# es_event_mmap_t

A type for an event that indicates the mapping of memory to a file.

Mac CatalystmacOS

``` source
struct es_event_mmap_t
```

## Topics

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The file to map memory into.

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

### Initializers

init(protection: Int32, max_protection: Int32, flags: Int32, file_pos: UInt64, source: UnsafeMutablePointer&lt;es_file_t>, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Memory Mapping Event Types

struct es_event_mprotect_t

A type for an event that indicates a change to protection of memory-mapped pages.

