

- Endpoint Security
-  es_mute_process(\_:\_:) 

Function

# es_mute_process(\_:\_:)

Suppresses events from a given process.

macOS 10.15+

``` source
func es_mute_process(
    _ client: OpaquePointer,
    _ audit_token: UnsafePointer
) -> es_return_t
```

## Parameters 

`client`  

A previously-created client. If the call succeeds, this client no longer receives events from the process indicated by `audit_token`.

`audit_token`  

The audit token that indicates the process to mute.

## Return Value

A value that indicates whether the mute request succeeded or failed with an error.

## Discussion

To mute a subset of events from a process, use es_mute_process_events(_:_:_:_:).

## See Also

### Muting Events

func es_mute_process_events(OpaquePointer, UnsafePointer&lt;audit_token_t>, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Suppresses a subset of events from a given process.

struct es_muted_processes_t

A structure for a set of muted processes.

func es_release_muted_processes(UnsafeMutablePointer&lt;es_muted_processes_t>)

Frees resources associated with a set of previously-retrieved muted processes.

func es_muted_processes_events(OpaquePointer, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_muted_processes_t>?>) -> es_return_t

Retrieve a list of all muted processes.

func es_mute_path(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t) -> es_return_t

Suppresses events from executables that match a given path.

func es_mute_path_events(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Suppresses a subset of events from executables that match a given path.

struct es_mute_path_type_t

The type of a path argument, such as a prefix or a path literal.

func es_muted_paths_events(OpaquePointer, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_muted_paths_t>>?) -> es_return_t

Retrieve a list of all muted paths.

struct es_muted_paths_t

A structure for a set of muted paths.

func es_release_muted_paths(UnsafeMutablePointer&lt;es_muted_paths_t>)

Frees resources associated with a set of previously-retrieved muted paths.

