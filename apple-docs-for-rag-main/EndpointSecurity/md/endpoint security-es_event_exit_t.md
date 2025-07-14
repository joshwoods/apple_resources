

- Endpoint Security
-  es_event_exit_t 

Structure

# es_event_exit_t

A type for an event that indicates a process exiting.

Mac CatalystmacOS

``` source
struct es_event_exit_t
```

## Topics

### Inspecting Event Properties

var stat: Int32

The exit status of the process.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init()

init(stat: Int32, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Process Event Types

struct es_event_chdir_t

A type for an event that indicates a change to a process’s working directory.

struct es_event_chroot_t

A type for an event that indicates a change to a process’s root directory.

struct es_event_exec_t

A type for an event that indicates the execution of a process.

struct es_event_fork_t

A type for an event that indicates the forking of a process.

struct es_event_proc_check_t

A type that indicates the call used and the data returned when a process checks on the access of the target process.

struct es_event_signal_t

A type for an event that indicates the sending of a signal to a process.

