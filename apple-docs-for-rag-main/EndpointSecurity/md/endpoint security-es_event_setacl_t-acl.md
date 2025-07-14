

- Endpoint Security
- es_event_setacl_t
-  acl 

Instance Property

# acl

A union containing a settable access control list structure.

Mac CatalystmacOS

``` source
var acl: es_event_setacl_t.__Unnamed_union_acl
```

## Discussion

The `acl` union is valid only when the set_or_clear value is ES_SET. In this case, the union contains an `acl_t` called `set` containing the access control list values.

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file containing the access control list to set or clear.

var set_or_clear: es_set_or_clear_t

The access control list action represented by the event, either setting or clearing values.

struct es_set_or_clear_t

A type that indicates whether an event represents setting or clearing a file’s access control list.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

