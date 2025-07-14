

- Endpoint Security
-  es_mute_process_events(\_:\_:\_:\_:) 

Function

# es_mute_process_events(\_:\_:\_:\_:)

Suppresses a subset of events from a given process.

macOS 12.0+

``` source
func es_mute_process_events(
    _ client: OpaquePointer,
    _ audit_token: UnsafePointer,
    _ events: UnsafePointer,
    _ event_count: Int
) -> es_return_t
```

## Parameters 

`client`  

A previously-created client. If the call succeeds, this client no longer receives events that match the types in the `events` array from the process indicated by `audit_token`.

`audit_token`  

The audit token that indicates the process to mute.

`events`  

An array of event types to mute.

`event_count`  

The number of members in the `events` array.

## Return Value

A value that indicates whether the mute request succeeded or failed with an error.

## Discussion

To mute all events from a process, use es_mute_process(_:_:).

## See Also

### Muting Events

func es_mute_process(OpaquePointer, UnsafePointer&lt;audit_token_t>) -> es_return_t

Suppresses events from a given process.

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

