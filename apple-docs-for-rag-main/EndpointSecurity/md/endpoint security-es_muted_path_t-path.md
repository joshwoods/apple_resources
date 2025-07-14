

- Endpoint Security
- es_muted_path_t
-  path 

Instance Property

# path

The muted path.

Mac CatalystmacOS

``` source
var path: es_string_token_t
```

## See Also

### Accessing Muted Path Properties

var type: es_mute_path_type_t

The path type: prefix or literal.

struct es_mute_path_type_t

The type of a path argument, such as a prefix or a path literal.

var events: UnsafePointer&lt;es_event_type_t>!

An array containing the muted event types.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

var event_count: Int

The number of elements in the muted events array.

struct es_string_token_t

A pointer to a null-terminated string, and the length in bytes of that string.

