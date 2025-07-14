

- Endpoint Security
-  es_muted_paths_t 

Structure

# es_muted_paths_t

A structure for a set of muted paths.

Mac CatalystmacOS

``` source
struct es_muted_paths_t
```

## Topics

### Accessing Muted Paths

var paths: UnsafePointer&lt;es_muted_path_t>!

An array containing the muted paths.

struct es_muted_path_t

A structure that describes a path’s muted events.

var count: Int

The number of elements in the paths array.

### Initializers

init()

init(count: Int, paths: UnsafePointer&lt;es_muted_path_t>!)

## Relationships

### Conforms To

- BitwiseCopyable

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

func es_muted_paths_events(OpaquePointer, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_muted_paths_t>>?) -> es_return_t

Retrieve a list of all muted paths.

func es_release_muted_paths(UnsafeMutablePointer&lt;es_muted_paths_t>)

Frees resources associated with a set of previously-retrieved muted paths.

