

- Endpoint Security
- es_event_clone_t
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

The file to clone.

var target_dir: UnsafeMutablePointer&lt;es_file_t>

The directory that contains the cloned file.

var target_name: es_string_token_t

The name of the newly cloned file.

