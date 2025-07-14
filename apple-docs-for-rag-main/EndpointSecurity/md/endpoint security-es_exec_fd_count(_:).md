

- Endpoint Security
-  es_exec_fd_count(\_:) 

Function

# es_exec_fd_count(\_:)

Gets the number of file descriptors from a process execution event.

macOS 11.0+

``` source
func es_exec_fd_count(_ event: UnsafePointer) -> UInt32
```

## Parameters 

`event`  

The process execution event.

## Return Value

The number of file descriptors.

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

struct es_fd_t

A structure that describes an open file descriptor.

