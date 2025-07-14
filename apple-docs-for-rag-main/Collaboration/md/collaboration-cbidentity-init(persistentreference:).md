

- Collaboration
- CBIdentity
-  init(persistentReference:) 

Initializer

# init(persistentReference:)

Returns the identity object matching the persistent reference data.

macOS 10.5+

``` source
init?(persistentReference data: Data)
```

## Parameters 

`data`  

The persistent data object that refers to an identity.

## Return Value

The identity object matching the persistent data object, or `nil` if the identity is not found.

## Discussion

A persistent reference is an opaque data object suitable for persistent storage.

## See Also

### Finding Identities

init?(name: String, authority: CBIdentityAuthority)

Returns the identity object with the given name from the specified identity authority.

init?(uuidString: String, authority: CBIdentityAuthority)

Returns the identity object with the given UUID from the specified identity authority.

Deprecated

