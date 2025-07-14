

- Assignables
-  UserIdentityFactory 

Enumeration

# UserIdentityFactory

A type that contains helpers for creating user identity objects.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum UserIdentityFactory
```

## Topics

### Getting the anonymous identity

static var anonymous: AnonymousUserIdentity

The anonymous user identity.

### Creating an identity

static func string(String) -> StringUserIdentity

Creates a StringUserIdentity with the given string value.

## See Also

### Identity

protocol UserIdentity

Types conforming to this protocol can act as user identities for editors of a document.

struct AnonymousUserIdentity

A user identity for unknown editors.

struct AnyUserIdentity

A user identity that performs type erasure by wrapping another user identity.

struct StringUserIdentity

A user identity defined by a string.

class UserIdentityTypeRegistry

A registry for user identity types. Assignable documents and document elements store user identity data as `Data` objects. In order for that data to be deserialized, the type to deserialize it as needs to be known to UserIdentityTypeRegistry. Without registration of the user identity, custom types won’t be deserializable.

