

- Endpoint Security
-  es_set_or_clear_t 

Structure

# es_set_or_clear_t

A type that indicates whether an event represents setting or clearing a file’s access control list.

Mac CatalystmacOS

``` source
struct es_set_or_clear_t
```

## Topics

### Event Types

var ES_CLEAR: es_set_or_clear_t

A case that indicates the event represents a clearing of the access control list.

var ES_SET: es_set_or_clear_t

A case that indicates the event represents a setting of access control list values.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file containing the access control list to set or clear.

var acl: es_event_setacl_t.__Unnamed_union_acl

A union containing a settable access control list structure.

var set_or_clear: es_set_or_clear_t

The access control list action represented by the event, either setting or clearing values.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

