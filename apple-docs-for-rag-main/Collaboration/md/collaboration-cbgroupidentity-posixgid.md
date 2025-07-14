

- Collaboration
- CBGroupIdentity
-  posixGID 

Instance Property

# posixGID

Returns the POSIX GID of the identity.

macOS 10.5+

``` source
var posixGID: gid_t { get }
```

## Return Value

The POSIX GID of the group identity.

## Discussion

The POSIX GID is an integer that can identify a group within an identity authority. GIDs are not guaranteed to be unique within an identity authority.

