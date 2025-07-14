

- Endpoint Security
-  es_unmute_all_paths(\_:) 

Function

# es_unmute_all_paths(\_:)

Restores event delivery from previously-muted paths.

macOS 10.15+

``` source
func es_unmute_all_paths(_ client: OpaquePointer) -> es_return_t
```

## Parameters 

`client`  

The client for which to unmute events.

## See Also

### Unmuting Events

func es_unmute_process(OpaquePointer, UnsafePointer&lt;audit_token_t>) -> es_return_t

Restores event delivery from a previously-muted process.

func es_unmute_process_events(OpaquePointer, UnsafePointer&lt;audit_token_t>, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted process.

func es_unmute_path(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t) -> es_return_t

Restores event delivery from a previously-muted path.

func es_unmute_path_events(OpaquePointer, UnsafePointer&lt;CChar>, es_mute_path_type_t, UnsafePointer&lt;es_event_type_t>, Int) -> es_return_t

Restores event delivery of a subset of events from a previously-muted path.

struct es_mute_path_type_t

The type of a path argument, such as a prefix or a path literal.

