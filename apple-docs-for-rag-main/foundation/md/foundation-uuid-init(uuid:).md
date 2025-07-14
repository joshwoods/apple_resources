

- Foundation
- UUID
-  init(uuid:) 

Initializer

# init(uuid:)

Creates a UUID from the uuid C-language structure.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(uuid: uuid_t)
```

## Parameters 

`uuid`  

The C-language structure of a UUID.

## See Also

### Creating UUIDs

init()

Creates a UUID with RFC 4122 version 4 random bytes.

init?(uuidString: String)

Creates a UUID from a string representation.

