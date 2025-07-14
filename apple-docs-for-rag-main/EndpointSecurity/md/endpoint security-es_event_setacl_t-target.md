

- Endpoint Security
- es_event_setacl_t
-  target 

Instance Property

# target

The file containing the access control list to set or clear.

Mac CatalystmacOS

``` source
var target: UnsafeMutablePointer
```

## See Also

### Inspecting Event Properties

var acl: es_event_setacl_t.__Unnamed_union_acl

A union containing a settable access control list structure.

var set_or_clear: es_set_or_clear_t

The access control list action represented by the event, either setting or clearing values.

struct es_set_or_clear_t

A type that indicates whether an event represents setting or clearing a file’s access control list.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

