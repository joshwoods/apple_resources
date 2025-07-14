

- Endpoint Security
-  es_event_exec_t 

Structure

# es_event_exec_t

A type for an event that indicates the execution of a process.

Mac CatalystmacOS

``` source
struct es_event_exec_t
```

## Overview

To get the process’ arguments, file descriptors, and environment variables from this type, use the following functions:

- Arguments — es_exec_arg(_:_:) and es_exec_arg_count(_:).

- Environment variables — es_exec_env(_:_:), and es_exec_env_count(_:).

- File descriptors — es_exec_fd(_:_:), es_exec_fd_count(_:).

## Topics

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process to execute.

struct es_process_t

A type that describes a process, as delivered by an Endpoint Security message.

### Instance Properties

var cwd: UnsafeMutablePointer&lt;es_file_t>

var dyld_exec_path: es_string_token_t

var image_cpusubtype: cpu_subtype_t

var image_cputype: cpu_type_t

var last_fd: Int32

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

var script: UnsafeMutablePointer&lt;es_file_t>?

## See Also

### Process Event Types

struct es_event_chdir_t

A type for an event that indicates a change to a process’s working directory.

struct es_event_chroot_t

A type for an event that indicates a change to a process’s root directory.

struct es_event_fork_t

A type for an event that indicates the forking of a process.

struct es_event_proc_check_t

A type that indicates the call used and the data returned when a process checks on the access of the target process.

struct es_event_signal_t

A type for an event that indicates the sending of a signal to a process.

struct es_event_exit_t

A type for an event that indicates a process exiting.

