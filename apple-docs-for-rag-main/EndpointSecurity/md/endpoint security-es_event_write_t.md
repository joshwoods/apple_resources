

- Endpoint Security
-  es_event_write_t 

Structure

# es_event_write_t

A type for an event that indicates the writing of data to a file.

Mac CatalystmacOS

``` source
struct es_event_write_t
```

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The source file of the event.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(target: UnsafeMutablePointer&lt;es_file_t>, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### File-System Event Types

struct es_file_t

A type that represents a file related to an Endpoint Security event.

struct es_event_access_t

A type for an event that indicates the checking of a file’s access permission.

struct es_event_clone_t

A type for an event that indicates the cloning of a file.

struct es_event_copyfile_t

A type for an event that indicates the copying of a file by use of a system call.

struct es_event_create_t

A type for an event that indicates the creation of a file.

struct es_event_dup_t

A type for an event that indicates the duplication of a file descriptor.

struct es_event_fcntl_t

A type for an event that indicates the manipulation of a file descriptor.

struct es_event_open_t

A type for an event that indicates the opening of a file.

struct es_event_close_t

A type for an event that indicates the closing of a file.

struct es_event_rename_t

A type for an event that indicates the renaming of a file.

struct es_event_truncate_t

A type for an event that indicates the truncation of a file.

struct es_event_exchangedata_t

A type for an event that indicates the exchange of data between two files.

struct es_event_lookup_t

A type for an event that indicates the lookup of a file’s path.

struct es_event_searchfs_t

A type for an event that indicates searching a volume or mounted file system.

