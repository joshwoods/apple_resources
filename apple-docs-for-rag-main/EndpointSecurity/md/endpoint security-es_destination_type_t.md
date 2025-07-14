

- Endpoint Security
-  es_destination_type_t 

Structure

# es_destination_type_t

A type that indicates how a file event presents its destination to the client.

Mac CatalystmacOS

``` source
struct es_destination_type_t
```

## Overview

Use this type to determine how to parse file information in types like es_event_create_t and es_event_rename_t. Both of those types have a `destination` member, which is a `union` of either an existing file path or a parent directory and name of a potential file. To determine which member of the union to access, consult the event’s `destination_type` member, which is of this type.

## Topics

### Destination Types

var ES_DESTINATION_TYPE_EXISTING_FILE: es_destination_type_t

The destination is an existing file.

var ES_DESTINATION_TYPE_NEW_PATH: es_destination_type_t

The destination is a path to a new location.

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

var destination: es_event_create_t.__Unnamed_union_destination

The file system destination of the created file.

var destination_type: es_destination_type_t

The type of destination for the event, which can be either an existing file or information that describes a new file’s pending location.

var reserved2: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

