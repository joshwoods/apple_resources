

- Endpoint Security
- es_event_create_t
-  destination 

Instance Property

# destination

The file system destination of the created file.

Mac CatalystmacOS

``` source
var destination: es_event_create_t.__Unnamed_union_destination
```

## Discussion

To parse this `union`, check the destination_type to determine whether the file already exists:

- If the destination_type is ES_DESTINATION_TYPE_EXISTING_FILE, the union contains an es_file_t member called `existing_file`.

- If the destination_type is ES_DESTINATION_TYPE_NEW_PATH, the union contains a `struct` called `new_path`, indicating the file’s proposed destination. The structure consists of an es_file_t called `dir` for the parent directory, an es_string_token_t called `filename`, and a mode_t called `mode`.

## See Also

### Inspecting Event Properties

var destination_type: es_destination_type_t

The type of destination for the event, which can be either an existing file or information that describes a new file’s pending location.

struct es_destination_type_t

A type that indicates how a file event presents its destination to the client.

var reserved2: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

