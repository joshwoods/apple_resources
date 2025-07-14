

- Endpoint Security
-  es_unmute_path(\_:\_:\_:) 

Function

# es_unmute_path(\_:\_:\_:)

Restores event delivery from a previously-muted path.

macOS 12.0+

``` source
func es_unmute_path(
    _ client: OpaquePointer,
    _ path: UnsafePointer,
    _ type: es_mute_path_type_t
) -> es_return_t
```

## Parameters 

`client`  

A previously-muted client. If the call succeeds, this client begins to receive events from executables whose paths match `path`.

`path`  

The path to unmute. The client resumes receiving events from executables whose paths match this string.

`type`  

The type of the `path` argument, either a prefix or a literal path.

## Return Value

A value that indicates whether the unmute request succeeded or failed with an error.

## Discussion

To unmute a subset of events from a path, use es_unmute_path_events(_:_:_:_:_:).

## See Also

### Unmuting Events

func es_unmute_process(OpaquePointer, UnsafePointer&lt;audit_token_t>) -> es_return_t

Restores event delivery from a previously-muted process.

func es_unmute_process_events(OpaquePointer, UnsafePointer&lt;audit_token_t>, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted process.

func es_unmute_path_events(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted path.

struct es_mute_path_type_t

The type of a path argument, such as a prefix or a path literal.

func es_unmute_all_paths(OpaquePointer) -> es_return_t

Restores event delivery from previously-muted paths.

