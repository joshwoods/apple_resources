

- Endpoint Security
- es_event_rename_t
-  destination 

Instance Property

# destination

The destination of the rename operation.

Mac CatalystmacOS

``` source
var destination: es_event_rename_t.__Unnamed_union_destination
```

## Discussion

To parse this `union`, check the destination_type to determine whether the rename event’s destination file already exists:

- If the destination_type is ES_DESTINATION_TYPE_EXISTING_FILE, the union contains an es_file_t member called `existing_file`.

- If the destination_type is ES_DESTINATION_TYPE_NEW_PATH, the union contains a `struct` called `new_path`, indicating the file’s proposed destination. The structure consists of an es_file_t called `dir` for the parent directory, and an es_string_token_t called `filename`.

## See Also

### Inspecting Event Properties

var source: UnsafeMutablePointer&lt;es_file_t>

The source file to rename.

var destination_type: es_destination_type_t

A property that indicates whether the destination is a new path or an existing file.

struct es_destination_type_t

A type that indicates how a file event presents its destination to the client.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

