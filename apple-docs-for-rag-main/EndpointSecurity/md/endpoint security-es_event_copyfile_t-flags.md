

- Endpoint Security
- es_event_copyfile_t
-  flags 

Instance Property

# flags

The flags argument of the system call.

Mac CatalystmacOS

``` source
var flags: Int32
```

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The file to clone.

var target_file: UnsafeMutablePointer&lt;es_file_t>?

The file, if any, that exists at the target location.

var target_dir: UnsafeMutablePointer&lt;es_file_t>

The directory that contains the copied file.

var target_name: es_string_token_t

The name of the newly copied file.

var mode: mode_t

The mode argument of the system call.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

