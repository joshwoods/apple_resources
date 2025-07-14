

- Endpoint Security
-  es_file_t 

Structure

# es_file_t

A type that represents a file related to an Endpoint Security event.

Mac CatalystmacOS

``` source
struct es_file_t
```

## Topics

### Inspecting File Properties

var path: es_string_token_t

The file’s path.

var path_truncated: Bool

A Boolean value that indicates whether Endpoint Security truncated the path string.

var stat: stat

The file’s metadata, such as file size, user and group identifiers, and access and modification dates.

### Initializers

init()

init(path: es_string_token_t, path_truncated: Bool, stat: stat)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### File-System Event Types

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

struct es_event_write_t

A type for an event that indicates the writing of data to a file.

struct es_event_lookup_t

A type for an event that indicates the lookup of a file’s path.

struct es_event_searchfs_t

A type for an event that indicates searching a volume or mounted file system.

