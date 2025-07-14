

- Collaboration
- CBIdentity
-  init(uuidString:authority:) Deprecated

Initializer

# init(uuidString:authority:)

Returns the identity object with the given UUID from the specified identity authority.

macOS 10.5–10.11Deprecated

``` source
init?(
    uuidString uuid: String,
    authority: CBIdentityAuthority
)
```

Deprecated

Use +identityWithUniqueIdentifier:authority: instead.

## Parameters 

`uuid`  

The UUID of the identity you are searching for.

`authority`  

The identity authority to search.

## Return Value

The identity object, or `nil` if no identity is found with the matching criteria.

## See Also

### Finding Identities

init?(name: String, authority: CBIdentityAuthority)

Returns the identity object with the given name from the specified identity authority.

init?(persistentReference: Data)

Returns the identity object matching the persistent reference data.

