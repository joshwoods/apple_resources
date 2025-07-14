

- Endpoint Security
-  es_event_setuid_t 

Structure

# es_event_setuid_t

A type for an event that indicates the setting of a process’s user ID.

Mac CatalystmacOS

``` source
struct es_event_setuid_t
```

## Topics

### Inspecting Event Properties

var uid: uid_t

The user ID.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init()

init(uid: uid_t, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### User and Group ID Types

struct es_event_setgid_t

A type for an event that indicates the setting of a process’s group ID.

struct es_event_seteuid_t

A type for an event that indicates the setting of a process’s effective user ID.

struct es_event_setegid_t

A type for an event that indicates the setting of a process’s effective group ID.

struct es_event_setreuid_t

A type for an event that indicates the setting of a process’s real and effective user IDs.

struct es_event_setregid_t

A type for an event that indicates the setting of a process’s real and effective group IDs.

