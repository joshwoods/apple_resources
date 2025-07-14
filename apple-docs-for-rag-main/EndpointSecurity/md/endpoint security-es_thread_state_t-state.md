

- Endpoint Security
- es_thread_state_t
-  state 

Instance Property

# state

The machine-specific thread state.

Mac CatalystmacOS

``` source
var state: es_token_t
```

## Discussion

This equivalent to thread_state_t in Mach APIs.

Note

The size subfield of the state field is in bytes, not natural_t units.

## See Also

### Inspecting Thread State

var flavor: Int32

An indication of the representation of the machine-specific thread state.

struct es_token_t

An arbitrary buffer of data with its size.

