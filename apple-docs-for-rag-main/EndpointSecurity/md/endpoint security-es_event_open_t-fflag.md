

- Endpoint Security
- es_event_open_t
-  fflag 

Instance Property

# fflag

The file-opening mask as applied by the kernel.

Mac CatalystmacOS

``` source
var fflag: Int32
```

## Discussion

This mask differs from the `oflag` values used in `open(2)`. When responding to this event, use `FFLAG` values such as `FREAD` and `FWRITE` instead, rather than `O_RDONLY`, `O_RDWR` and the like.

## See Also

### Inspecting Event Properties

var file: UnsafeMutablePointer&lt;es_file_t>

The file to open.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

