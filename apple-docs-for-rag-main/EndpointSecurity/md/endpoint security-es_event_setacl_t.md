

- Endpoint Security
-  es_event_setacl_t 

Structure

# es_event_setacl_t

A type for an event that indicates the setting of a file’s access control list.

Mac CatalystmacOS

``` source
struct es_event_setacl_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file containing the access control list to set or clear.

var acl: es_event_setacl_t.__Unnamed_union_acl

A union containing a settable access control list structure.

var set_or_clear: es_set_or_clear_t

The access control list action represented by the event, either setting or clearing values.

struct es_set_or_clear_t

A type that indicates whether an event represents setting or clearing a file’s access control list.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(target: UnsafeMutablePointer&lt;es_file_t>, set_or_clear: es_set_or_clear_t, acl: es_event_setacl_t.__Unnamed_union_acl, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

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

struct es_event_readdir_t

A type for an event that indicates the reading of a file-system directory.

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

