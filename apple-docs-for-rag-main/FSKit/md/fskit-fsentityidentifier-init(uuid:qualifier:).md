

- FSKit
- FSEntityIdentifier
-  init(uuid:qualifier:) 

Initializer

# init(uuid:qualifier:)

Creates an entity identifier with the given UUID and qualifier data as a 64-bit unsigned integer.

macOS 15.4+

``` source
init(
    uuid: UUID,
    qualifier: UInt64
)
```

## Parameters 

`uuid`  

The UUID to use for this identifier.

`qualifier`  

The data to distinguish entities that otherwise share the same UUID.

## See Also

### Creating an entity identifier

init()

Creates an entity identifier with a random UUID.

init(uuid: UUID)

Creates an entity identifier with the given UUID.

init(uuid: UUID, data: Data)

Creates an entity identifier with the given UUID and qualifier data.

