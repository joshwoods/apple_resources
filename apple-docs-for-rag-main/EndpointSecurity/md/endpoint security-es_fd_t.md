

- Endpoint Security
-  es_fd_t 

Structure

# es_fd_t

A structure that describes an open file descriptor.

Mac CatalystmacOS

``` source
struct es_fd_t
```

## Topics

### Inspecting File Descriptor Properties

var fd: Int32

The file descriptor number.

var fdtype: UInt32

The file descriptor type, as a libproc type.

### Initializers

init()

### Instance Properties

var pipe: es_fd_t.__Unnamed_union___Anonymous_field2.__Unnamed_struct_pipe

## Relationships

### Conforms To

- Sendable

## See Also

### Process Event Helper Functions

func es_exec_arg(UnsafePointer&lt;es_event_exec_t>, UInt32) -> es_string_token_t

Gets the argument at the specified position from a process execution event.

func es_exec_arg_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of arguments from a process execution event.

func es_exec_env(UnsafePointer&lt;es_event_exec_t>, UInt32) -> es_string_token_t

Gets the environment variable at the specified position from a process execution event.

func es_exec_env_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of environment variables from a process execution event.

func es_exec_fd(UnsafePointer&lt;es_event_exec_t>, UInt32) -> UnsafePointer&lt;es_fd_t>

Gets the file descriptor at the specified position from a process execution event.

func es_exec_fd_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of file descriptors from a process execution event.

