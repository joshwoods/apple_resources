

- Endpoint Security
-  es_exec_arg(\_:\_:) 

Function

# es_exec_arg(\_:\_:)

Gets the argument at the specified position from a process execution event.

macOS 10.15+

``` source
func es_exec_arg(
    _ event: UnsafePointer,
    _ index: UInt32
) -> es_string_token_t
```

## Parameters 

`event`  

The process execution event.

`index`  

The zero-based index of the argument to return. Attempting to read an out-of-bounds index — where `index >= es_exec_arg_count()` — results in undefined behavior.

## Return Value

A string token that contains the argument data and its length.

## Discussion

This function doesn’t allocate memory for the returned token; it points to a string token inside of `event`. Because you don’t own this memory, don’t try to free it.

Warning

The returned pointer must not outlive the `event` parameter passed to the function, because the pointer will likely be invalid after the function returns.

## See Also

### Process Event Helper Functions

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

struct es_fd_t

A structure that describes an open file descriptor.

