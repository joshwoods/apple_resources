

- Foundation
- UUID
-  init(uuidString:) 

Initializer

# init(uuidString:)

Creates a UUID from a string representation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(uuidString string: String)
```

## Parameters 

`string`  

The string representation of a UUID, such as `E621E1F8-C36C-495A-93FC-0C247A3E6E5F`.

## Discussion

Returns `nil` if the string isn’t a valid UUID representation.

## See Also

### Creating UUIDs

init()

Creates a UUID with RFC 4122 version 4 random bytes.

init(uuid: uuid_t)

Creates a UUID from the uuid C-language structure.

