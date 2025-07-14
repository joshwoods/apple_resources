

- Assignables
- StringUserIdentity
-  UserIdentity Implementations 

API Collection

# UserIdentity Implementations

## Topics

### Instance Methods

func eraseToAnyUserIdentity() -> AnyUserIdentity

Wraps this user identity with a type eraser.

func scope&lt;R>(() async throws -> R) async rethrows -> R

Sets the user identity for document-related operations that occur within the async closure passed in.

func scope&lt;R>(() throws -> R) rethrows -> R

Sets the user identity for document-related operations that occur within the closure passed in.

### Type Aliases

typealias As

An alias for UserIdentityFactory for convenience.

