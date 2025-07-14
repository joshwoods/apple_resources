

- Endpoint Security
-  es_event_fork_t 

Structure

# es_event_fork_t

A type for an event that indicates the forking of a process.

Mac CatalystmacOS

``` source
struct es_event_fork_t
```

## Topics

### Inspecting Event Properties

var child: UnsafeMutablePointer&lt;es_process_t>

The forked child process.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

### Initializers

init(child: UnsafeMutablePointer&lt;es_process_t>, reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Process Event Types

struct es_event_chdir_t

A type for an event that indicates a change to a process’s working directory.

struct es_event_chroot_t

A type for an event that indicates a change to a process’s root directory.

struct es_event_exec_t

A type for an event that indicates the execution of a process.

struct es_event_proc_check_t

A type that indicates the call used and the data returned when a process checks on the access of the target process.

struct es_event_signal_t

A type for an event that indicates the sending of a signal to a process.

struct es_event_exit_t

A type for an event that indicates a process exiting.

