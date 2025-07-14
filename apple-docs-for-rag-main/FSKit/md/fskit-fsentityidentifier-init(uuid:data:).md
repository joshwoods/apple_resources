

- FSKit
- FSEntityIdentifier
-  init(uuid:data:) 

Initializer

# init(uuid:data:)

Creates an entity identifier with the given UUID and qualifier data.

macOS 15.4+

``` source
init(
    uuid: UUID,
    data qualifierData: Data
)
```

## Parameters 

`uuid`  

The UUID to use for this identifier.

`qualifierData`  

The data to distinguish entities that otherwise share the same UUID.

## See Also

### Creating an entity identifier

init()

Creates an entity identifier with a random UUID.

init(uuid: UUID)

Creates an entity identifier with the given UUID.

init(uuid: UUID, qualifier: UInt64)

Creates an entity identifier with the given UUID and qualifier data as a 64-bit unsigned integer.

