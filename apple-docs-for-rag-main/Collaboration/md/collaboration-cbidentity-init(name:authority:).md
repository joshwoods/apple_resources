

- Collaboration
- CBIdentity
-  init(name:authority:) 

Initializer

# init(name:authority:)

Returns the identity object with the given name from the specified identity authority.

macOS 10.5+

``` source
init?(
    name: String,
    authority: CBIdentityAuthority
)
```

## Parameters 

`name`  

The name of the identity.

`authority`  

The identity authority to search.

## Return Value

The identity object, or `nil` if no identity is found with the specified name.

## Discussion

The name is compared against all valid identity names, including full names, short names, email addresses, and aliases.

## See Also

### Finding Identities

init?(persistentReference: Data)

Returns the identity object matching the persistent reference data.

init?(uuidString: String, authority: CBIdentityAuthority)

Returns the identity object with the given UUID from the specified identity authority.

Deprecated

