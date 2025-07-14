

- Endpoint Security
- es_event_remote_thread_create_t
-  thread_state 

Instance Property

# thread_state

The new thread’s state.

Mac CatalystmacOS

``` source
var thread_state: UnsafeMutablePointer?
```

## Discussion

When creating a thread with `thread_create_running(_:_:_:_:_:)`, this value contains an es_thread_state_t value. When using `thread_create(_:_:)`, this value is `NULL`.

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process targeted to spawn a new thread.

struct es_thread_state_t

A description of a thread’s machine-specfiic state.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

