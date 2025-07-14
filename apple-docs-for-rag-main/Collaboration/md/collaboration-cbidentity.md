

- Collaboration
-  CBIdentity 

Class

# CBIdentity

A `CBIdentity` object is used for accessing the attributes of an identity stored in an identity authority. You can use an identity object for finding identities, and storing them in an access control list (ACL). If you need to edit these attributes, take advantage of the `CSIdentity` class in Core Services.

macOS 10.5+

``` source
class CBIdentity
```

## Overview

You can obtain a `CBIdentity` object from one of the following class factory methods: init(name:authority:), init(uuidString:authority:), init(persistentReference:), or identityWithCSIdentity:.

A `CBIdentity` object has methods to support for interoperability with the Core Services Identity API. Send CSIdentity to your `CBIdentity` object to return an opaque object for use in the Core Services Identity API. Similarly, call identityWithCSIdentity: to use an Core Services Identity opaque object in the Collaboration framework.

There are two subclasses of `CBIdentity`: `CBGroupIdentity` and `CBUserIdentity`. If you are working specifically with a group identity, use `CBGroupIdentity`. Similarly, if you are working with a user identity, use `CBUserIdentity`.

## Topics

### Finding Identities

init?(name: String, authority: CBIdentityAuthority)

Returns the identity object with the given name from the specified identity authority.

init?(persistentReference: Data)

Returns the identity object matching the persistent reference data.

init?(uuidString: String, authority: CBIdentityAuthority)

Returns the identity object with the given UUID from the specified identity authority.

Deprecated

### Getting Identity Attributes

var aliases: [String]

Returns an array of aliases (alternate names) for the identity.

var authority: CBIdentityAuthority

Returns the identity authority where the identity is stored.

var emailAddress: String?

Returns the email address of an identity.

var fullName: String

Returns the full name of the identity.

var image: NSImage?

Returns the image associated with an identity.

var isHidden: Bool

Returns a Boolean value indicating the state of the identity’s hidden property.

func isMember(ofGroup: CBGroupIdentity) -> Bool

Returns a Boolean value indicating whether the identity is a member of the specified group.

var posixName: String

Returns the POSIX name of the identity.

var uuidString: String

Returns the UUID of the identity as a string.

Deprecated

### Storing Identities

var persistentReference: Data?

Returns a persistent reference to store a reference to an identity.

### Initializers

init?(uniqueIdentifier: UUID, authority: CBIdentityAuthority)

### Instance Properties

var uniqueIdentifier: UUID

## Relationships

### Inherits From

- NSObject

### Inherited By

- CBGroupIdentity
- CBUserIdentity

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

