

- Endpoint Security
-  es_mute_path_prefix(\_:\_:) Deprecated

Function

# es_mute_path_prefix(\_:\_:)

Suppresses events from executables matching a path prefix.

macOS 10.15–12.0Deprecated

``` source
func es_mute_path_prefix(
    _ client: OpaquePointer,
    _ path_prefix: UnsafePointer
) -> es_return_t
```

Deprecated

Use es_mute_path(_:_:_:) or es_mute_path_events(_:_:_:_:_:) instead.

## Parameters 

`client`  

The client for which to mute events.

`path_prefix`  

A prefix string. The client stops receiving events from executables whose paths begin with this string.

## See Also

### Deprecated Functions

func es_muted_processes(OpaquePointer, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;audit_token_t>>?) -> es_return_t

Generates a list of muted processes.

Deprecated

func es_mute_path_literal(OpaquePointer, UnsafePointer&lt;CChar>) -> es_return_t

Suppresses events from executables matching a path literal.

Deprecated

