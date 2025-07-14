

- Endpoint Security
-  es_event_link_t 

Structure

# es_event_link_t

A type for an event that indicates the creation of a hard link.

Mac CatalystmacOS

``` source
struct es_event_link_t
```

## Topics

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The source file for the link.

var target_dir: UnsafeMutablePointer&lt;es_file_t>

The directory that contains the newly-created link.

var target_filename: es_string_token_t

The file name of the symbolic link.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(source: UnsafeMutablePointer&lt;es_file_t>, target_dir: UnsafeMutablePointer&lt;es_file_t>, target_filename: es_string_token_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Link Event Types

struct es_event_readlink_t

A type for an event that indicates the reading of a symbolic link.

struct es_event_unlink_t

A type for an event that indicates the deletion of a file.

