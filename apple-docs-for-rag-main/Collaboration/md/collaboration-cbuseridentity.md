

- Collaboration
-  CBUserIdentity 

Class

# CBUserIdentity

An object of the `CBUserIdentity` class represents a user identity and is used for accessing the attributes of a user identity from an identity authority. The principal attributes of `CBUserIdentity` are a POSIX user identifier (UID), password, and certificate.

macOS 10.5+

``` source
class CBUserIdentity
```

## Topics

### Password Authentication

func authenticate(withPassword: String) -> Bool

Returns a Boolean value indicating whether the given password is correct for the identity.

var certificate: SecCertificate?

Returns the public authentication certificate associated with a user identity.

var isEnabled: Bool

Returns a Boolean value indicating whether the identity is allowed to authenticate.

### Using UIDs

var posixUID: uid_t

Returns the POSIX UID of the identity.

init?(posixUID: uid_t, authority: CBIdentityAuthority)

Returns the user identity with the given POSIX UID in the specified identity authority.

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

