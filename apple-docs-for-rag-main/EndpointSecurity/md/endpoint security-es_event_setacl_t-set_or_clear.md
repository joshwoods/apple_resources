

- Endpoint Security
- es_event_setacl_t
-  set_or_clear 

Instance Property

# set_or_clear

The access control list action represented by the event, either setting or clearing values.

Mac CatalystmacOS

``` source
var set_or_clear: es_set_or_clear_t
```

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file containing the access control list to set or clear.

var acl: es_event_setacl_t.__Unnamed_union_acl

A union containing a settable access control list structure.

struct es_set_or_clear_t

A type that indicates whether an event represents setting or clearing a file’s access control list.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

