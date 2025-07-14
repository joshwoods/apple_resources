

- Endpoint Security
- es_event_link_t
-  reserved 

Instance Property

# reserved

An unused field reserved for future use.

Mac CatalystmacOS

``` source
var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)
```

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The source file for the link.

var target_dir: UnsafeMutablePointer&lt;es_file_t>

The directory that contains the newly-created link.

var target_filename: es_string_token_t

The file name of the symbolic link.

