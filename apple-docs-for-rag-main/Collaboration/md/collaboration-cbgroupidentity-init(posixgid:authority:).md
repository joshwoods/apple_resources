

- Collaboration
- CBGroupIdentity
-  init(posixGID:authority:) 

Initializer

# init(posixGID:authority:)

Returns the group identity with the given POSIX GID in the specified identity authority.

macOS 10.5+

``` source
init?(
    posixGID gid: gid_t,
    authority: CBIdentityAuthority
)
```

## Parameters 

`gid`  

The GID of the group identity you are searching for.

`authority`  

An identity authority in which to search for the group identity.

## Return Value

The group identity object with the given GID in the specified identity authority, or `nil` if no identity exists with the specified GID.

## See Also

### Related Documentation

Identity Services Programming Guide

