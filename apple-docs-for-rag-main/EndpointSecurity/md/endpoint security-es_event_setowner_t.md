

- Endpoint Security
-  es_event_setowner_t 

Structure

# es_event_setowner_t

A type for an event that indicates the setting of a file’s owner.

Mac CatalystmacOS

``` source
struct es_event_setowner_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file with ownership metadata to set.

var uid: uid_t

The user identifier to set.

var gid: gid_t

The group identifier to set.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(uid: uid_t, gid: gid_t, target: UnsafeMutablePointer&lt;es_file_t>, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

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

struct es_event_readdir_t

A type for an event that indicates the reading of a file-system directory.

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

struct es_event_stat_t

A type for an event that indicates the retrieval of a file’s status.

struct es_event_utimes_t

A type for an event that indicates a change to a file’s access time or modification time.

