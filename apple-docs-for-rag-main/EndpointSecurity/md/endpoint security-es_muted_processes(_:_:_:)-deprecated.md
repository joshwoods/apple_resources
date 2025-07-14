

- Endpoint Security
-  es_muted_processes(\_:\_:\_:) Deprecated

Function

# es_muted_processes(\_:\_:\_:)

Generates a list of muted processes.

macOS 10.15–12.0Deprecated

``` source
func es_muted_processes(
    _ client: OpaquePointer,
    _ count: UnsafeMutablePointer,
    _ audit_tokens: UnsafeMutablePointer>?
) -> es_return_t
```

Deprecated

Use es_muted_processes_events(_:_:) instead.

## Parameters 

`client`  

The client for which to generate a list of muted proceses.

`count`  

On return, the number of audit tokens generated.

`audit_tokens`  

On return, an array of audit tokens, each of which represents a muted process.

## Return Value

A value that indicates whether the request succeeded or failed with an error.

## Discussion

The caller handles freeing the memory pointed to by `audit_token`.

## See Also

### Deprecated Functions

func es_mute_path_literal(OpaquePointer, UnsafePointer&lt;CChar>) -> es_return_t

Suppresses events from executables matching a path literal.

Deprecated

func es_mute_path_prefix(OpaquePointer, UnsafePointer&lt;CChar>) -> es_return_t

Suppresses events from executables matching a path prefix.

Deprecated

