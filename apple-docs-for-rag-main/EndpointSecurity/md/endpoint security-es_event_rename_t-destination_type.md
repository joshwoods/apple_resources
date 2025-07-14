

- Endpoint Security
- es_event_rename_t
-  destination_type 

Instance Property

# destination_type

A property that indicates whether the destination is a new path or an existing file.

Mac CatalystmacOS

``` source
var destination_type: es_destination_type_t
```

## Discussion

Use this property to determine how to access the destination field.

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The source file to rename.

var destination: es_event_rename_t.__Unnamed_union_destination

The destination of the rename operation.

struct es_destination_type_t

A type that indicates how a file event presents its destination to the client.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

