

- Endpoint Security
- es_event_copyfile_t
-  target_file 

Instance Property

# target_file

The file, if any, that exists at the target location.

Mac CatalystmacOS

``` source
var target_file: UnsafeMutablePointer?
```

## Discussion

The copy file operation overwrites this file if the operation completes. If no file exists at the target location, this value is `NULL`.

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The file to clone.

var target_dir: UnsafeMutablePointer&lt;es_file_t>

The directory that contains the copied file.

var target_name: es_string_token_t

The name of the newly copied file.

var mode: mode_t

The mode argument of the system call.

var flags: Int32

The flags argument of the system call.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

