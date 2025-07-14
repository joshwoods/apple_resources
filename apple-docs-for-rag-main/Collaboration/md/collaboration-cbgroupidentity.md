

- Collaboration
-  CBGroupIdentity 

Class

# CBGroupIdentity

An object of the `CBGroupIdentity` class represents a group identity and is used for viewing the attributes of group identities from an identity authority. The principal attributes of a `CBGroupIdentity` object are a POSIX group identifier (GID) and a list of members.

macOS 10.5+

``` source
class CBGroupIdentity
```

## Topics

### Finding Group Identities

init?(posixGID: gid_t, authority: CBIdentityAuthority)

Returns the group identity with the given POSIX GID in the specified identity authority.

### Group Identity Attributes

var posixGID: gid_t

Returns the POSIX GID of the identity.

### Instance Properties

var memberIdentities: [CBIdentity]

## Relationships

### Inherits From

- CBIdentity

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

