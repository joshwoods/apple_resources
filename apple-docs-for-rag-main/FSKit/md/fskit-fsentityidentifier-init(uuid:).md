

- FSKit
- FSEntityIdentifier
-  init(uuid:) 

Initializer

# init(uuid:)

Creates an entity identifier with the given UUID.

macOS 15.4+

``` source
init(uuid: UUID)
```

## Parameters 

`uuid`  

The UUID to use for this identifier.

## See Also

### Creating an entity identifier

init()

Creates an entity identifier with a random UUID.

init(uuid: UUID, data: Data)

Creates an entity identifier with the given UUID and qualifier data.

init(uuid: UUID, qualifier: UInt64)

Creates an entity identifier with the given UUID and qualifier data as a 64-bit unsigned integer.

