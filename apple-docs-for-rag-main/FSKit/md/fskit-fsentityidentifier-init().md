

- FSKit
- FSEntityIdentifier
-  init() 

Initializer

# init()

Creates an entity identifier with a random UUID.

macOS 15.4+

``` source
init()
```

## See Also

### Creating an entity identifier

init(uuid: UUID)

Creates an entity identifier with the given UUID.

init(uuid: UUID, data: Data)

Creates an entity identifier with the given UUID and qualifier data.

init(uuid: UUID, qualifier: UInt64)

Creates an entity identifier with the given UUID and qualifier data as a 64-bit unsigned integer.

