

- Endpoint Security
-  es_event_mount_t 

Structure

# es_event_mount_t

A type for an event that indicates the mounting of a file system.

Mac CatalystmacOS

``` source
struct es_event_mount_t
```

## Topics

### Inspecting Event Properties

var statfs: UnsafeMutablePointer&lt;statfs>

The statistics of the mounted file system.

typealias es_statfs_t

A type that represents statistics about a file system.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(statfs: UnsafeMutablePointer&lt;statfs>, disposition: es_mount_disposition_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

### Instance Properties

var disposition: es_mount_disposition_t

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### File System Mounting Event Types

struct es_event_unmount_t

A type for an event that indicates the unmounting of a file system.

struct es_event_remount_t

A type for an event that indicates the unmounting of a file system.

