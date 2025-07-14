

- Endpoint Security
- es_event_create_t
-  destination_type 

Instance Property

# destination_type

The type of destination for the event, which can be either an existing file or information that describes a new file’s pending location.

Mac CatalystmacOS

``` source
var destination_type: es_destination_type_t
```

## Discussion

Use the value of this member to parse the destination union.

## See Also

### Inspecting Event Properties

var destination: es_event_create_t.__Unnamed_union_destination

The file system destination of the created file.

struct es_destination_type_t

A type that indicates how a file event presents its destination to the client.

var reserved2: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

