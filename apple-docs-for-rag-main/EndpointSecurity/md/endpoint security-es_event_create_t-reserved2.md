

- Endpoint Security
- es_event_create_t
-  reserved2 

Instance Property

# reserved2

An unused field reserved for future use.

Mac CatalystmacOS

``` source
var reserved2: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)
```

## See Also

### Inspecting Event Properties

var destination: es_event_create_t.__Unnamed_union_destination

The file system destination of the created file.

var destination_type: es_destination_type_t

The type of destination for the event, which can be either an existing file or information that describes a new file’s pending location.

struct es_destination_type_t

A type that indicates how a file event presents its destination to the client.

