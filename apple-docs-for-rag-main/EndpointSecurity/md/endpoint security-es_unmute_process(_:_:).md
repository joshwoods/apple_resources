

- Endpoint Security
-  es_unmute_process(\_:\_:) 

Function

# es_unmute_process(\_:\_:)

Restores event delivery from a previously-muted process.

macOS 10.15+

``` source
func es_unmute_process(
    _ client: OpaquePointer,
    _ audit_token: UnsafePointer
) -> es_return_t
```

## Parameters 

`client`  

A previously-muted client. If the call succeeds, this client begins to receive events from the process indicated by `audit_token`.

`audit_token`  

The audit token indicating the process to unmute.

## Return Value

A value that indicates whether the unmute request succeeded or failed with an error.

## Discussion

To unmute a subset of events from a process, use es_unmute_process_events(_:_:_:_:).

## See Also

### Unmuting Events

func es_unmute_process_events(OpaquePointer, UnsafePointer&lt;audit_token_t>, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted process.

func es_unmute_path(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t) -> es_return_t

Restores event delivery from a previously-muted path.

func es_unmute_path_events(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted path.

struct es_mute_path_type_t

The type of a path argument, such as a prefix or a path literal.

func es_unmute_all_paths(OpaquePointer) -> es_return_t

Restores event delivery from previously-muted paths.

