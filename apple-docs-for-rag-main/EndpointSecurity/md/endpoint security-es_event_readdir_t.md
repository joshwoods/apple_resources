

- Endpoint Security
-  es_event_readdir_t 

Structure

# es_event_readdir_t

A type for an event that indicates the reading of a file-system directory.

Mac CatalystmacOS

``` source
struct es_event_readdir_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The directory from which to read contents.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(target: UnsafeMutablePointer&lt;es_file_t>, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### File Metadata Event Types

struct es_event_deleteextattr_t

A type for an event that indicates the deletion of an extended attribute from a file.

struct es_event_fsgetpath_t

A type for an event that indicates the retrieval of a file-system path.

struct es_event_getattrlist_t

A type for an event that indicates the retrieval of attributes from a file.

struct es_event_getextattr_t

A type for an event that indicates the retrieval of an extended attribute from a file.

struct es_event_listextattr_t

A type for an event that indicates the retrieval of multiple extended attributes from a file.

struct es_event_setacl_t

A type for an event that indicates the setting of a file’s access control list.

struct es_event_setattrlist_t

A type for an event that indicates the setting of a file attribute.

struct es_event_setextattr_t

A type for an event that indicates the setting of a file’s extended attribute.

struct es_event_setflags_t

A type for an event that indicates the setting of a file’s flags.

struct es_event_setmode_t

A type for an event that indicates the setting of a file’s mode.

struct es_event_setowner_t

A type for an event that indicates the setting of a file’s owner.

struct es_event_stat_t

A type for an event that indicates the retrieval of a file’s status.

struct es_event_utimes_t

A type for an event that indicates a change to a file’s access time or modification time.

