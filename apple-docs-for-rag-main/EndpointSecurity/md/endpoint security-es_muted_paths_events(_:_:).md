

- Endpoint Security
-  es_muted_paths_events(\_:\_:) 

Function

# es_muted_paths_events(\_:\_:)

Retrieve a list of all muted paths.

macOS 12.0+

``` source
func es_muted_paths_events(
    _ client: OpaquePointer,
    _ muted_paths: UnsafeMutablePointer>?
) -> es_return_t
```

## Parameters 

`client`  

A previously-created client. If the call succeeds, the `muted_paths` structure contains paths muted for this client.

`muted_paths`  

On output, a structure that contains the muted paths. You must dispose of this memory by calling es_release_muted_paths(_:).

## Return Value

A value that indicates whether the request for muted paths succeeded or failed with an error.

## See Also

### Muting Events

func es_mute_process(OpaquePointer, UnsafePointer&lt;audit_token_t>) -> es_return_t

Suppresses events from a given process.

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

struct es_muted_paths_t

A structure for a set of muted paths.

func es_release_muted_paths(UnsafeMutablePointer&lt;es_muted_paths_t>)

Frees resources associated with a set of previously-retrieved muted paths.

